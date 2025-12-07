# 🔡 Languages

## 📁 Subdirectories

- [Script Languages](script-languages/script-languages.md)
- [System Languages](system-languages/system-languages.md)
- [Web Languages](web-languages/web-languages.md)

---
## 📄 Files
---
1. [🔡 Languages](#-languages)
   1. [📁 Subdirectories](#-subdirectories)
   2. [📄 Files](#-files)
      1. [🧩 정규표현식이란(Regular Expressions)?](#-정규표현식이란regular-expressions)
         1. [🔑 기본 문법 핵심](#-기본-문법-핵심)
         2. [📌 기억하기 쉽게 하는 방법](#-기억하기-쉽게-하는-방법)
         3. [🏋️ 연습 문제](#️-연습-문제)
      2. [🛢️ JSON (Java Script Object Notation)](#️-json-java-script-object-notation)
         1. [🔑 Primary Purpose of JSON](#-primary-purpose-of-json)
         2. [📐 JSON Syntax and Structure](#-json-syntax-and-structure)
            1. [1. Objects (`{}`)](#1-objects-)
            2. [2. Arrays (`[]`)](#2-arrays-)
            3. [Supported Data Types (Values)](#supported-data-types-values)
---

### 🧩 정규표현식이란(Regular Expressions)?
- **문자열 패턴을 찾는 언어**예요.  
- “조건에 맞는 문자열을 걸러내는 필터”라고 생각하면 쉽습니다. 
- 예: 이메일 주소, 전화번호, 특정 단어 찾기 등.
---
#### 🔑 기본 문법 핵심
| 기호 | 의미                    | 예시    | 매칭 결과        |
| ---- | ----------------------- | ------- | ---------------- |
| `.`  | 아무 문자 1개           | `a.b`   | `acb`, `a1b`     |
| `*`  | 앞 문자가 0회 이상 반복 | `ab*`   | `a`, `ab`, `abb` |
| `+`  | 앞 문자가 1회 이상 반복 | `ab+`   | `ab`, `abb`      |
| `?`  | 앞 문자가 0회 또는 1회  | `ab?`   | `a`, `ab`        |
| `[]` | 문자 집합               | `[abc]` | `a`, `b`, `c`    |
| `^`  | 문자열 시작             | `^abc`  | `abc...`         |
| `$`  | 문자열 끝               | `xyz$`  | `...xyz`         |
| `\d` | 숫자                    | `\d\d`  | `12`, `99`       |
| `\w` | 알파벳/숫자/밑줄        | `\w+`   | `hello_123`      |
| `\s` | 공백 문자               | `\s+`   | 띄어쓰기, 탭     |

---
#### 📌 기억하기 쉽게 하는 방법
1. **의미 단위로 묶어라**  
   - `\d{3}-\d{4}-\d{4}` → 전화번호 패턴  
   - `{n}`은 “정확히 n번 반복”이라는 규칙.
2. **자주 쓰는 패턴을 예시로 외워라**  
   - 이메일: `\w+@\w+\.\w+`  
   - 우편번호(5자리): `^\d{5}$`
3. **테스트하면서 학습**  
   - [regex101.com](https://regex101.com) 같은 사이트에서 직접 입력해보면 바로 매칭 결과가 보여서 이해가 빨라요.
---
#### 🏋️ 연습 문제
제가 간단한 퀴즈를 내볼게요.  
- 패턴: `^a.*z$`  
👉 어떤 문자열들이 매칭될까요?  

힌트: 시작은 `a`, 끝은 `z`, 중간엔 뭐든 올 수 있음.  

### 🛢️ JSON (Java Script Object Notation)
---
**JSON** stands for **JavaScript Object Notation**. 
It is a **lightweight data-interchange format** that is very easy for humans to read and write, and simple for machines to parse and generate.

#### 🔑 Primary Purpose of JSON
---
The main purpose of JSON is to **transmit structured data** across a network, typically between a **server** and a **web application** (client).

It has become the dominant format used by almost all modern **APIs (Application Programming Interfaces)** due to its simplicity and efficiency compared to older formats like XML.

  * **Language-Independent:** Although its syntax is based on JavaScript object notation, JSON is completely language-independent. Most programming languages (Python, Java, C\#, etc.) have built-in libraries to easily read (parse) and write (stringify) JSON data.
  * **Data Structure:** It is built on two universal data structures that are familiar to almost all modern programming languages:
    1.  A collection of **name/value pairs** (called an **object**).
    2.  An **ordered list of values** (called an **array**).

-----

#### 📐 JSON Syntax and Structure

JSON data is structured using two main components:

##### 1\. Objects (`{}`)

An object is an unordered collection of **key/value pairs**. This is used to represent an entity or record.

  * It begins and ends with **curly braces** (`{}`).
  * Each key is a **string** (must be enclosed in **double quotes**).
  * The key and value are separated by a **colon** (`:`).
  * Pairs are separated by a **comma** (`,`).

<!-- end list -->

```json
{
  "firstName": "John",
  "lastName": "Doe",
  "isStudent": false
}
```

##### 2\. Arrays (`[]`)

An array is an ordered list of values. This is used to represent a list of records or repeating data.

  * It begins and ends with **square brackets** (`[]`).
  * Values are separated by a **comma** (`,`).
  * The values in an array can be of different types, including other objects or arrays (allowing for nested data).

<!-- end list -->

```json
[
  "apple",
  "banana",
  "cherry"
]
```

##### Supported Data Types (Values)
The value in a key/value pair or an array element can be one of the following six types:
  * **String:** A sequence of characters (must be in double quotes).
  * **Number:** Integer or floating-point.
  * **Boolean:** `true` or `false`.
  * **Object:** Another JSON object (`{}`).
  * **Array:** Another JSON array (`[]`).
  * **`null`:** An empty value.


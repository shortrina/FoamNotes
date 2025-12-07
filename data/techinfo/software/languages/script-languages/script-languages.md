---
foam_template:
  filepath: "techinfo/software/languages/script-languages/script-languages.md"
  description: "what is script languages"
---

# 📝 script-languages
>[!NOTE]
> A scripting language is a type of programming language that provides instructions for a runtime environment, such as a web browser or operating system shell. Unlike conventional programming languages like C or C++, scripting languages are generally interpreted at runtime rather than being compiled into machine code beforehand.
> 
> <u>**Key Characteristics**</u>
> > **Interpreted**: Code is translated and executed line-by-line by an interpreter when the script is run, rather than all at once by a compiler before execution. This allows for faster development and testing cycles.
> > **Runtime Environment:** Scripts typically run within an existing host program or environment (e.g., a web browser, server, or game engine) and automate tasks or enhance the functionality of that parent software.
> > **Automation & Integration:** They are often used for automating repetitive tasks, generating dynamic web content, or "gluing" together more complex software components.
> > **Simpler Syntax:** Scripting languages often have a more concise and readable syntax, making them easier for beginners to learn.
>
>  <u>**Common Examples**</u>
> Some of the most widely used scripting languages include:
> > **JavaScript:** Primarily used for client-side web development to create dynamic and interactive user experiences within web browsers. It can also be used for server-side development via Node.js.
> > **Python:** A general-purpose language popular for web development, data analysis, automation, and system administration due to its simplicity and robust libraries.
> > **PHP:** A server-side scripting language designed specifically for web development and creating dynamic web pages.
> > **Ruby:** A dynamic, object-oriented language known for its clear and simple syntax, often used with the Ruby on Rails web framework.
> > **Bash:** A command language interpreter for the Linux operating system, used for shell scripting and automating command-line tasks.

## 🐚 Shell
---
## 🐚 What is Shell Scripting?
---
A **Shell Script** is a computer program—specifically, a **scripting language**—designed to be run by a **Unix shell**, which is the command-line interpreter for Unix-like operating systems (such as Linux, macOS, and even specialized environments on Windows).

Think of the shell as the intermediary that translates your commands into actions the operating system (OS) can understand. A shell script is essentially a **text file containing a sequence of commands** that you would normally type manually into the terminal.

### Key Characteristics:

* **Interpreter-Based:** Shell scripts are *interpreted*, not compiled. The shell (like **Bash**, **Zsh**, or **Ksh**) reads and executes the commands one line at a time.
* **Command Automation:** It combines existing system utilities (`ls`, `cp`, `grep`, `awk`, `sed`, etc.) into a single, automated workflow.
* **Control Flow:** Like a regular programming language, shell scripts support **variables**, **conditional statements** (if/else), and **loops** (for/while), allowing for complex logic and decision-making.
* **The Shebang:** Almost every script starts with a special line called the **shebang** (e.g., `#!/bin/bash`), which tells the OS which interpreter program to use to run the script. 


## 🛠️ Why is Shell Scripting Used?
---
The primary purpose of shell scripting is **automation**. It allows system administrators, developers, and DevOps professionals to automate repetitive, routine, and complex system tasks efficiently, reducing human error.

### Common Use Cases:

| Area                      | Example Tasks                                                                                                                                                                |
| :------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **System Administration** | Automated **database backups**, system **log rotation**, monitoring disk space or CPU load, and user account management (creation/deletion).                                 |
| **Development & DevOps**  | Automating the **deployment** of software (copying files to servers), running **test suites**, building and packaging applications, and setting up development environments. |
| **File Management**       | Performing bulk operations like **renaming hundreds of files** based on a pattern, cleaning up old temporary files, or organizing data directories.                          |
| **Data Processing**       | Searching for patterns within large **log files** (`grep`), manipulating text data, and generating simple reports.                                                           |
| **Scheduling**            | Setting up tasks to run automatically at specific times (using tools like `cron`) for maintenance or reporting.                                                              |

In short, if a task involves running a series of system commands repeatedly or conditionally on a Unix-like operating system, a shell script is the fastest and most native way to do it.

This video gives an introduction to what shell scripting is and provides a tutorial for beginners. [Introduction to Shell Scripting | Shell Scripting Tutorial for Beginners](https://www.youtube.com/watch?v=RvYKa5S6BRY)


## 💻 JavaScript
---
### 💻 What is JavaScript?
---
**JavaScript (JS)** is a **scripting or programming language** that is one of the three core technologies of the World Wide Web, alongside **HTML** (which structures the content) and **CSS** (which styles the content).

It's primarily used as a **client-side scripting language**, meaning the code is executed directly in the user's web browser, but it can also be used for **server-side programming** (e.g., with Node.js). [Image of HTML CSS JavaScript logos showing their relationship]


### 💡 Why is JavaScript Needed?
---
JavaScript is essential because it allows developers to implement **complex and interactive features** on web pages, moving them beyond static displays of information.

The key need for JavaScript is to make websites **dynamic** and **responsive** to user actions.

- **Interactive Webpages:** It enables features like drop-down menus, image carousels, form validation, and animations. Anytime a web page _does_ something other than just displaying fixed text and images, JavaScript is likely involved.
- **Dynamic Content:** It can modify a webpage's content, layout, and style _after_ it has loaded. For instance, it can load new data without requiring a full-page refresh (often called AJAX).
- **User Experience (UX):** By handling user input and events (like mouse clicks or key presses), JavaScript significantly improves the user experience by making the interaction fluid and immediate.
- **Full-Stack Development:** With server-side runtimes like **Node.js**, JavaScript can be used for the back-end (server logic, database interaction) as well, making it a versatile language for developing complete web applications.

This video provides an explanation of what JavaScript is and its role: [What Is JavaScript and Why Do I Need It?](https://www.youtube.com/watch?v=KyuQyhUamug).
http://googleusercontent.com/youtube_content/0

## 📘 TypeScript
---
### 📘 What is TypeScript?
---
**TypeScript (TS)** is a programming language developed and maintained by Microsoft. It is a **strict syntactical superset of JavaScript**, which means:

1.  **Any valid JavaScript code is also valid TypeScript code.**
2.  TypeScript adds its own features on top of JavaScript, most importantly **Static Typing**.

TypeScript code cannot be run directly by a browser or Node.js. Instead, it must be **transpiled** (compiled) into plain JavaScript first.

The core difference is that TypeScript lets you explicitly define the **data type** of variables, function parameters, and return values (e.g., `string`, `number`, `boolean`).


### 🚀 Why Was TypeScript Developed and Used?
---
TypeScript was developed to solve the primary challenge of building **large-scale applications** using JavaScript: the lack of a strong type system.

JavaScript is **dynamically typed**, meaning it checks variable types only when the code is actually running (**at runtime**). This often leads to bugs that are hard to find.

TypeScript, on the other hand, introduces **static typing**, which means:

#### 1. Catching Errors Early (Type Safety)

- **Benefit:** Errors related to mixing up data types (like trying to treat a `string` as a `number`) are caught immediately by the compiler during the development phase (**compile-time**), not later when the application is running and a user encounters the issue.
  - _Example:_ If a function is supposed to take a number, TypeScript will flag an error immediately if you try to pass it a string.

#### 2. Scalability and Maintainability

- **Benefit:** As an application grows and the code base becomes huge, the explicit type definitions act as **documentation**.
  - It becomes much easier for new developers to understand what kind of data a function expects and what it returns without having to read the entire function's logic.
  - Refactoring (reorganizing code) is safer because the type-checker ensures that changes in one part of the code don't unexpectedly break another part.

#### 3. Better Developer Experience (Tooling)

- **Benefit:** The static type information allows modern code editors (like VS Code) to provide **smarter tooling**.
  - This includes powerful **autocompletion** (IntelliSense), **intelligent code navigation**, and instant feedback on errors as you type. This significantly boosts developer productivity.

In summary, while JavaScript is great for flexibility and smaller projects, **TypeScript is necessary for large, complex applications** because it adds a layer of robustness and safety, making the code more reliable, easier to manage, and less prone to runtime bugs.

---

## Node.js

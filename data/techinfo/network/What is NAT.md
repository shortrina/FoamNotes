# What is NAT?

Network Address Translation (NAT)는 라우터나 방화벽을 통해 네트워크 패킷의 헤더에 있는 IP 주소 정보를 수정하는 네트워킹 기술입니다.[1][2] NAT를 통해 개인 네트워크의 여러 장치가 **하나의 공용 IP 주소를 공유**하여 인터넷 같은 외부 네트워크와 통신할 수 있습니다.[2][3]

## NAT의 주요 목적

NAT는 주로 두 가지 중요한 목적으로 사용됩니다:[1][3] 먼저 **IPv4 주소 부족 문제를 해결**합니다. 제한된 공용 IP 주소를 효율적으로 사용하여 많은 내부 장치들이 하나의 공용 IP로 인터넷에 접근할 수 있습니다. 둘째, **내부 네트워크의 보안을 강화**하는데, 내부 IP 주소를 외부 네트워크로부터 숨김으로써 보호 계층을 제공합니다.[3]

## NAT의 작동 원리

NAT의 작동 방식은 다음과 같습니다:[2][4]

**발신 트래픽 (Source NAT)**: 개인 네트워크 내 장치가 인터넷 리소스에 요청을 보낼 때, NAT 라우터는 패킷의 출발지 IP 주소를 자신의 공용 IP 주소로 변경합니다.[2] 동시에 여러 내부 장치를 구분하기 위해 각 장치에 고유한 포트 번호를 할당합니다.[2]

**NAT 테이블 기록**: 라우터는 변환된 매핑 정보(내부 IP 주소, 원래 포트, 새로운 포트)를 NAT 테이블에 저장합니다.[1]

**응답 트래픽 (Destination NAT)**: 외부 서버로부터 응답이 돌아오면, 라우터는 NAT 테이블의 저장된 정보를 사용하여 어느 내부 장치로 보낼지 파악합니다.[2] 그 후 공용 IP와 포트를 원래의 개인 IP와 포트로 다시 변경하여 패킷을 내부 장치로 전달합니다.[2][4]

## NAT의 유형

**정적 NAT (Static NAT)**: 내부 IP 주소가 특정 공용 IP 주소로 고정적으로 매핑됩니다.[6] 웹 서버나 이메일 서버처럼 인터넷에서 항상 접근 가능해야 하는 서비스에 주로 사용됩니다.[6]

**동적 NAT (Dynamic NAT)**: 내부 IP 주소들이 공용 IP 주소 풀의 사용 가능한 주소로 동적으로 매핑됩니다.[6] 이는 일대다(one-to-many) 매핑 방식입니다.[6]

**포트 주소 변환 (PAT/NAPT)**: 여러 개인 IP 주소가 **하나의 공용 IP 주소로 매핑**되며, 포트 번호로 장치를 구분합니다.[2][5] 이는 가정용 라우터와 소규모 사무실에서 가장 흔하게 사용되는 유형입니다.[2]

## 실제 적용 예시

NAT는 가정의 Wi-Fi 라우터, 기업 방화벽, 클라우드 인프라 등 다양한 환경에서 사용됩니다.[5] 예를 들어 집에서 여러 기기(스마트폰, 노트북, 태블릿)가 하나의 인터넷 연결로 동시에 웹을 사용할 수 있는 것이 바로 NAT 덕분입니다.

NAT는 인터넷의 효율성을 높이고 네트워크 보안을 강화하는 필수적인 기술이 되었습니다.

출처 :
[1] https://en.wikipedia.org/wiki/Network_address_translation
[2] https://www.broadbandsearch.net/definitions/network-address-translation
[3] https://csrc.nist.gov/glossary/term/network_address_translation
[4] https://www.geeksforgeeks.org/computer-networks/network-address-translation-nat/
[5] https://www.cisco.com/site/us/en/learn/topics/networking/what-is-network-address-translation-nat.html
[6] https://www.fortinet.com/resources/cyberglossary/network-address-translation
[7] https://whatismyipaddress.com/nat
[8] https://www.vmware.com/topics/network-address-translation
[9] https://www.youtube.com/watch?v=FTUV0t6JaDA

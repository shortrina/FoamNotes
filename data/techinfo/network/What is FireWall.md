
# What is FireWall

네트워크 방화벽(Network Firewall)은 신뢰할 수 있는 내부 네트워크와 신뢰할 수 없는 외부 네트워크 사이의 트래픽을 필터링하는 **보안 장치 또는 소프트웨어**입니다.[1][2] 조직의 네트워크 경계에서 게이트키퍼 역할을 하며, 들어오고 나가는 모든 데이터 패킷을 검사하여 보안 정책에 따라 허용하거나 차단합니다.[1][2]

## 네트워크 방화벽의 작동 원리

네트워크 방화벽은 정해진 보안 규칙에 따라 각 데이터 패킷을 분석하여 작동합니다.[1] 출발지 및 목적지 IP 주소, 포트 번호, 프로토콜 유형 등 패킷의 다양한 특성을 평가하여 그 패킷의 정당성을 판단합니다.[2] 안전하고 권한이 있는 데이터만 통과시키고 잠재적으로 악의적인 트래픽은 차단합니다.[1]

현대의 고급 방화벽은 **상태 기반 검사(Stateful Inspection)**를 수행하여 활성 연결의 상태를 추적하고, **심층 패킷 검사(Deep Packet Inspection, DPI)**를 통해 패킷 내부의 데이터를 검사하여 숨겨진 위협을 찾아냅니다.[1][2]

## 주요 기능 및 역할

네트워크 방화벽은 조직의 네트워크 보안을 위해 여러 중요한 기능을 수행합니다:[4]

**접근 제어**: 방화벽은 네트워크에서 허용되어야 할 인바운드 및 아웃바운드 트래픽 유형을 규제합니다.[4] IP 주소, 도메인, 포트 번호 기반으로 트래픽을 필터링할 수 있습니다.[6]

**위협 방어**: 방화벽은 네트워크 리소스에 도달하기 전에 위협을 탐지하고 차단합니다.[4] 악성코드, 알려진 악성 IP 주소로부터의 접근, 미승인 원격 접근 시도를 막습니다.[5] 또한 랜섬웨어 공격을 방지하기 위해 명령 및 제어 서버와의 통신을 차단합니다.[5]

**네트워크 분할**: 방화벽은 더 큰 네트워크를 더 작고 제어된 세그먼트로 나누어 각 영역에 고유의 접근 제어를 설정합니다.[2] 이를 통해 민감한 정보와 시스템에 대한 접근 권한을 제한하여 공격 표면을 줄입니다.[2]

**로깅 및 감사**: 방화벽은 네트워크 활동을 상세히 기록하여 의심스러운 행동을 식별하고 보안 위협의 성격을 파악할 수 있도록 합니다.[2][4]

## 네트워크 방화벽의 중요성

네트워크 방화벽은 네트워크 보안의 **첫 번째 방어선**입니다.[1] 공격 표면을 단일 접촉점으로 좁혀, 네트워크의 모든 호스트가 인터넷에 직접 노출되는 것을 방지합니다.[3] 이를 통해 미승인 접근을 방지하고 바이러스, 웜, 해커 공격으로부터 네트워크를 보호하며, 내부 네트워크 시스템의 무결성과 기밀성을 유지합니다.[1][2]

## 주요 용도

네트워크 방화벽은 다양한 상황에서 활용됩니다:[2]

- 외부 위협(해커, 악성코드 등)으로부터의 보호
- 보안 정책 및 규정 준수 강제
- 원격 근무자를 위한 보안 VPN 연결 제공
- 규정 준수 및 감사 요구 사항 충족

네트워크 방화벽은 현대 조직의 필수적인 보안 구성 요소로, 조직이 사이버 위협으로부터 네트워크 인프라를 효과적으로 보호할 수 있게 해줍니다.

출처 :
[1] https://www.paloaltonetworks.com/cyberpedia/what-is-a-network-firewall
[2] https://nilesecure.com/network-security/network-firewall
[3] https://www.kaspersky.com/resource-center/definitions/firewall
[4] https://www.catonetworks.com/network-firewall/
[5] https://www.barracuda.com/support/glossary/network-firewall
[6] https://www.checkpoint.com/cyber-hub/network-security/what-is-network-firewall/
[7] https://www.cisco.com/site/us/en/learn/topics/security/what-is-a-firewall.html
[8] https://www.fortinet.com/resources/cyberglossary/firewall
[9] https://en.wikipedia.org/wiki/Firewall_(computing)

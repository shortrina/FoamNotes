# What is DDNS?

Dynamic DNS (DDNS)는 IP 주소가 변경될 때마다 DNS 레코드를 자동으로 업데이트하는 서비스입니다.[1][2] 이를 통해 자주 변하는 IP 주소를 가진 장치나 서비스도 일관된 도메인 이름으로 접근할 수 있게 됩니다.

## DDNS의 필요성

대부분의 인터넷 서비스 제공자(ISP)는 가정용 고객이나 소규모 사업체에 **동적 IP 주소**를 할당합니다.[2] 고정 IP 주소는 비용이 비싸기 때문입니다. 그러나 웹 서버나 모니터링 장치처럼 인터넷을 통해 지속적으로 접근해야 하는 서비스를 운영하려면, IP 주소가 변경되어도 같은 도메인 이름으로 접근할 수 있어야 합니다. 이때 DDNS가 매우 유용합니다.[3]

## DDNS의 작동 원리

DDNS의 작동 방식은 다음과 같습니다:[4]

1. DDNS 제공자에 도메인 이름을 등록하고 현재 IP 주소와 연결합니다.
2. 로컬 장치나 라우터에서 실행되는 DDNS 클라이언트가 공용 IP 주소를 모니터링합니다.
3. IP 주소가 변경되면 클라이언트가 DDNS 제공자에 알립니다.
4. 제공자가 DNS 레코드를 업데이트하여 도메인이 올바른 IP를 가리키도록 합니다.
5. 이 과정이 지속적으로 반복되어 도메인과 IP가 항상 동기화 상태를 유지합니다.

## 주요 장점

**자동화**: 관리자가 매번 DNS 레코드를 수동으로 변경할 필요가 없습니다.[3] DDNS는 모든 업데이트를 자동으로 처리하므로 시간과 인력을 절약할 수 있습니다.

**실시간 접근성**: 서비스는 IP 주소가 변경되어도 중단 없이 접근 가능합니다.[3]

**비용 효율성**: 고정 IP 주소를 구입하지 않고도 안정적인 도메인 이름 기반의 접근이 가능합니다.

## 활용 사례

- **원격 모니터링**: 보안 카메라나 모니터링 장치에 도메인 이름을 할당하여 IP 변경에도 안정적으로 원격 접근 가능[3]
- **클라우드 인스턴스 관리**: 멀티클라우드 환경에서 의미 있는 호스트명을 할당[3]
- **재해복구 및 페일오버**: 주 서버 장애 시 빠르게 트래픽을 백업 서버로 리다이렉트[3]

DDNS는 특히 동적 IP를 할당받는 가정용 네트워크나 소규모 사업체가 온라인 서비스를 운영할 때 매우 실용적인 솔루션입니다.

출처 :
[1] https://www.cloudns.net/blog/what-is-dynamic-dns/
[2] https://en.wikipedia.org/wiki/Dynamic_DNS
[3] https://www.fortinet.com/resources/cyberglossary/dynamic-dns
[4] https://www.paloaltonetworks.com/cyberpedia/what-is-dynamic-dns
[5] https://www.cloudflare.com/learning/dns/glossary/dynamic-dns/
[6] https://www.cbtnuggets.com/blog/technology/networking/what-is-ddns
[7] https://www.youtube.com/watch?v=rOLGvZagdC0

### 동적 라우팅 프로토콜인 IGP(Interior Gateway Protocol) 와 EGP(Exterior Gateway Protocol)를 설명하시오.
**1. 동적 라우팅 프로토콜 IGP 와 EGP 관계 설명**
- [IGP] <---동일 조직 내부망--- [관리영역] ---다른조직 ISP간---> [EGP]

**2. 내부망 프로토콜, IGP(Interior Gateway Protocol) 설명**
- 가) IGP(Interior Gateway Protocol) 개념
    - 단일 관리 영여(동일 조직 또는 내부망) 내의 라우터들끼리 라우팅 정보를 교환해 네트워크 경로를 결정하는 프로토콜.

- 나) IGP(Interior Gateway Protocol) 기술요소

|구분|기술요소|설명|
|:------|:-------------|:------|
|프로토콜|RIP|거리 벡터 라우팅 방식의 대표 프로토콜|
|프로토콜|OSPF|링크 상태(Link state) 라우팅 방식|
|프로토콜|EIGRP|Cisco 독자 기술 기반의 하이브리드 라우팅 프로토콜|
|라우팅방식|Distance Vector|단순 최대 흡수 제한|
|라우팅방식|Link State|복잡, 빠르고 안정적인 경로 수립|
|라우팅방식|Hybrid|빠른 수렴성, 효율적 경로 탐색 제공|
|테이블갱신|Dynamic Update|네트워크 변경 시 자동으로 라우팅 테이블 갱신|

**3. 외부망 프로토콜,EGP(Exterior Gateway Protocol) 설명**
- 가) EGP(Exterior Gateway Protocol) 개념
    - 여러 개의 관리영역(서로 다른 조직이나 isp간) 간 라우터들이 경계 정보를 교환하기 위한 프로토콜.

- 나) EGP(Exterior Gateway Protocol) 기술요소

|구분|기술요소|설명|
|:------|:-------------|:------|
|프로토콜|BGP(Border Gateway Protocol)|목적지까지의 경로를  각 AS의 목록형태로 관리하여 루프방지가 가능|
|라우팅방식|정책 기반 라우팅|단순 최단 경로가 아닌, 다양한 정책(경로제어,보안,우선순위)에 따라 경로 결정|
|통신방식|유니캐스트|TCP 포토 179번 사용|
|적용 대상|글로벌 인터넷 수준|대규모 인터넷 환경에서 수십만 경로를 효율적으로 처리하며, 수렴 속도는 느리지만 안정성이 매우 높음|

```고도의 안정성 및 정책 제어 필요한 외부 네트워크 연결에 적용```

## 1) NECR-CIP란? 
#### NECR-CIP (North American Electric Reliabilty Corporation - Critical Infrastructure Protection)
북미 전력 신뢰성 공사(NECR)가 제정한 전력망(전력 산업) 사이버 보안 표준
전력 시스템 (발전소, 변전소, 제어센터 등)의 정보 인프라를 보호하기 위한 보안 규정 세트

## 2) 핵심 목적
- 전력 시스템을 운영하는 중요 자산 (ICS, SCADA, 제어 네트워크 등)을 식별하고 이에 대한 접근 통제, 네트워크 보안, 변경관리, 로그감시, 사고대응 등을 표준화
**사이버 위협으로부터 전력 인프라 보호** 

## 3) 주요 표준 구성 (CIP Standards)
| CIP 번호 | 주요 내용 | 명확한 실행 조치 | 예시 |
|-----------|------------|------------------|------|
| **CIP-002** | **BES 사이버 시스템 분류 (Categorization)**<br>BES에 영향을 줄 수 있는 사이버 자산을 식별하고 등급(High/Medium/Low) 분류 | - BMS, SCADA, EMS 등 핵심 시스템과 직접 통신하는 서버는 별도 서버라도 **BCA 또는 PCA**로 분류해야 함.<br>- 통신 대상의 등급을 상속(예: BMS가 Medium → Historian 서버도 Medium).<br>- 분류 근거를 문서화하고 정기적 재평가 수행. | - 발전소, 변전소, 제어센터, 통신 장비 등 시스템 자산 목록 작성<br>- 각 자산이 전력망 안정성(BES)에 미치는 영향도 평가<br>- “High Impact BES Cyber System” 등급 지정 |
| **CIP-003** | **보안 관리 및 정책 (Security Management Controls)**<br>보안 정책 수립, 책임자 지정, 거버넌스 체계 마련 | - **CIP 책임자(CIP Senior Manager)** 지정 및 문서화.<br>- 보안정책 수립·배포 후 연 1회 이상 검토.<br>- 외부 협력사 계약서에 CIP 준수 조항 명시.<br>- 정책 변경 기록(Log of Changes) 유지. | - 보안정책(Security Policy) 수립 및 주기적 검토<br>- 보안 책임자 지정<br>- 외부 협력사 및 벤더에 대한 보안 요구사항 명문화 |
| **CIP-004** | **인력 보안 및 교육 (Personnel & Training)**<br>중요 자산 접근 인력에 대한 신원검증, 교육 및 권한관리 | - 신규 인력 **배경조사(Background Check)** 수행.<br>- 연 1회 이상 **보안 인식 교육 (Security Training)** 실시.<br>- 퇴직·전보 시 접근권한 즉시 철회.<br>- 접근 가능 인력 목록 최신 유지. | - 접근 인력에 대한 신원 검증 기록<br>- 보안 인식 교육 수료증<br>- 퇴사자 접근 권한 철회 로그 |
| **CIP-005** | **전자적 보안 경계 (Electronic Security Perimeter)**<br>ESP 설정, 네트워크 접근 통제 및 외부 접속 제한 | - **내부 방화벽** 및 **EACMS** 구성.<br>- 외부 접근은 **DMZ → Jump Server → BMS** 순서로만 허용.<br>- **VPN + MFA** 인증 적용.<br>- 포트/프로토콜 제한 및 로그 보관. | - DMZ 및 방화벽 구성<br>- EACMS 운영<br>- 원격 접속 인증·로깅 |
| **CIP-006** | **물리적 보안 (Physical Security of BES Cyber Systems)**<br>제어실, 서버실 등 중요 설비의 물리적 출입통제 및 감시 | - 출입통제 시스템(카드, 생체 등) 설치.<br>- CCTV 및 침입감지 센서 운용.<br>- 방문자 관리 및 동행 정책 수립.<br>- 출입 로그 월 1회 검토. | - 서버실·제어실 출입통제 기록<br>- CCTV 녹화자료 보관<br>- 방문자 서명대장 |
| **CIP-007** | **시스템 보안 관리 (System Security Management)**<br>패치관리, 계정관리, 로그관리, 악성코드 방지 등 시스템 수준 보안 | - **보안 패치 주기(월 1회)** 설정 및 적용 기록 보관.<br>- 관리자 계정 공유 금지.<br>- 로그 중앙 수집(SIEM).<br>- 백신(AV/EDR) 최신화. | - 계정관리 로그<br>- 패치관리 리포트<br>- EDR 탐지 결과 |
| **CIP-008** | **사고 보고 및 대응 (Incident Reporting & Response)**<br>보안 사고 탐지·보고·대응 절차 수립 및 실행 | - **Incident Response Plan(IRP)** 작성 및 연 1회 모의훈련.<br>- 사고 분류 체계 정의.<br>- 사고 2시간 내 NERC 보고.<br>- 사후 분석(Lessons Learned) 기록. | - 사고 보고서<br>- 훈련 결과 보고서<br>- 사고 대응 로그 |
| **CIP-009** | **복구 계획 (Recovery Plans for BES Cyber Systems)**<br>장애 또는 사고 발생 시 시스템 복구 및 운영 연속성 확보 | - 정기 백업 및 복구 테스트(연 1회 이상).<br>- 백업본을 외부 안전 장소에 보관.<br>- 복구 절차 문서화 및 최신화.<br>- 복구 시 데이터 무결성 검증. | - 복구 시나리오 문서<br>- 백업 검증 리포트<br>- 복구 로그 |
| **CIP-010** | **구성 변경 및 취약점 관리 (Configuration & Vulnerability Management)**<br>시스템 및 네트워크 변경 통제, 취약점 평가 및 보완 | - 변경 시 **Change Request Form** 작성 및 승인.<br>- 변경 후 영향도 평가 실시.<br>- 정기 취약점 스캔(Nessus 등) 수행.<br>- 변경 내역을 Baseline 문서로 유지. | - 변경 승인 기록<br>- 취약점 보고서<br>- 구성 관리 문서 |
| **CIP-011** | **정보 보호 (Information Protection)**<br>중요 정보의 무단 접근·유출 방지, 암호화 및 폐기 절차 적용 | - 민감 정보 식별 및 등급 분류.<br>- 저장 시 AES-256 암호화, 전송 시 TLS 적용.<br>- Role-Based Access Control(RBAC) 정책 운영.<br>- 문서 폐기 시 디스크 완전 삭제. | - 암호화 정책 문서<br>- RBAC 접근 목록<br>- 폐기 로그 |



식별 -> 보호 -> 대응 -> 복구 -> 개선 과정을 아우르는 전력 인프라 보안의 완전한 수명주기 규정 세트

## 4) 미국 전력·에너지 프로젝트 데이터 보안 규제의 3대 축
### 4-1) NECR-CIP

### 4-2) Zero Trust Network
#### Zero Trust Network란?
"아무도, 아무 시스템도 기본적으로 신회하지 않는다."
네트워크 내부이든 외부든 모든 접근을 검증하고 최소한의 권한만 허용하는 모델

#### Zero Trust Network 핵심 원칙
- 모든 사용자가 위험하다고 항상 가정
- 네트워크에 외부 및 내부 위협이 항상 존재
- 모든 디바이스, 사용자, 네트워크 흐름을 인증하고 권한을 확인해야함
- 네트워크의 위치로 네트워크의 신뢰 여부를 결정할 수 없음
- 보안 제어 및 정책은 동적이고 가능한 많은 데이터 소스에서 계산되어야 함

### 4-3) CFIUS (Committee on Foreign Investment in the United States)
#### CFIUS (Committee on Foreign Investment in the United States)란?
미국 내 외국인 투자에 대한 국가안보 영향 심의 위원회
외국 기업이 미국 내 기업, 기술, 부동산, 에너지 시설 등에 투자·지분 취득·운영 참여할 때 그 행위가 미국의 국가 안보에 위협이 되는지 여부를 심사
#### CFIUS 심사 절차 요약
1. 사전 신고 (Voluntary Notice)
- 외국 이겁이 미국 내 투자 계획을 CFIUS에 자발적으로 신고
2. 초기 심사 (Review)
- 약 45일 내에 안보 위협 여부를 평가
3. 심층 조사 (Investigation)
- 위험이 있다고 판단되면 추가 45일 조사
4. 결정 (Decision)
- 조건부 승인, 구조조정 명령, 혹은 투자 금지 결정

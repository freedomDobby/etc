## 1) NECR-CIP란? 
#### NECR-CIP (North American Electric Reliabilty Corporation - Critical Infrastructure Protection)
북미 전력 신뢰성 공사(NECR)가 제정한 전력망(전력 산업) 사이버 보안 표준
전력 시스템 (발전소, 변전소, 제어센터 등)의 정보 인프라를 보호하기 위한 보안 규정 세트

## 2) 핵심 목적
- 전력 시스템을 운영하는 중요 자산 (ICS, SCADA, 제어 네트워크 등)을 식별하고 이에 대한 접근 통제, 네트워크 보안, 변경관리, 로그감시, 사고대응 등을 표준화
** 사이버 위협으로부터 전력 인프라 보호 ** 

## 3) 주요 표준 구성 (CIP Standards)
| CIP 번호      | 주요 내용                                                            |
| ----------- | ---------------------------------------------------------------- |
| **CIP-002** | 중요 자산 식별 (BES Cyber Assets Identification)                       |
| **CIP-003** | 보안 관리 및 정책(Security Management Controls)                         |
| **CIP-004** | 인력 보안 (Personnel & Training)                                     |
| **CIP-005** | 전자적 보안 경계 (Electronic Security Perimeter)                        |
| **CIP-006** | 물리적 보안 (Physical Security of BES Cyber Systems)                  |
| **CIP-007** | 시스템 보안 관리 (System Security Management)                           |
| **CIP-008** | 사고 대응 (Incident Reporting and Response)                          |
| **CIP-009** | 복구 계획 (Recovery Plans for BES Cyber Systems)                     |
| **CIP-010** | 구성 변경 및 취약점 관리 (Configuration Change & Vulnerability Management) |
| **CIP-011** | 정보 보호 (Information Protection)                                   |

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

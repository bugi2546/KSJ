## 프로젝트명: APT 전술 흐름을 구현한 시나리오 기반 포렌식 학습 플랫폼 설계
## 팀명: 짱돌
## 프로젝트 설명
### 간단 요약
1. 공격자가 짱돌 건설 회사를 장악하는 스토리
2. 현실성을 위해 실제 많이 발생하는 전술 선택
3. 공격자, 분석가, 통제자의 3대 관점을 모두 체험할 수 있는 플랫폼 설계

### 공격 시나리오
웹셸 업로드 → 영속성 확보 → 권한 상승 → AD 서버 장악 → GPO 악용을 통한 전사 백도어 설치 → 데이터 유출 → 랜섬웨어 배포

### MITRE ATT&CK 기반 전술 분류
1. Initial Access (T1190)
2. Execution (T1059)
3. Privilege Escalation (T1068)
4. Credential Access (T1003)
5. Lateral Movement (T1021.001)
6. Impact (T1486)

## 짱돌 건설 PC 정보 (가상 IP)
웹 서버:      	192.168.0.20
              192.168.100.20	  Windows Server 2019	   
              
AD 서버:	      192.168.100.10	  Windows Server 2019	  

DB 서버:	      192.168.100.30	  Windows Server 2019	   

파일 서버:	    192.168.100.40	  Windows Server 2019	   

Executive PC:	192.168.100.60	  Windows 10 Pro	       

CEO PC:	      192.168.100.25	  Windows 10 Pro	      

### 환경 구축에 사용된 도구
1. VMware
2. SQL ~
3. 

### 프로젝트의 산출물
1. 침해사고 분석 보고서
2.  ~ 침해사고 플랫폼
3.  


* 이 프로젝트는 학습용으로 설계되었으며, 다른 목적으로 사용 시 책임을 물을 수 있음. *

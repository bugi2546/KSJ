## 프로젝트명: APT 전술 흐름을 구현한 시나리오 기반 포렌식 학습 플랫폼 설계
## 팀명: 짱돌
## 프로젝트 설명
### 간단 요약
1. 공격자가 짱돌 건설 회사를 장악하는 스토리
2. 현실성과 몰입감을 구현하기 위해 실제 많이 발생하는 전술 선택

## APT 공격 시나리오
웹셸 업로드 → 영속성 확보 → 권한 상승 → AD 서버 장악 → GPO 악용을 통한 전사 백도어 설치 → 데이터 유출 → 랜섬웨어 배포

## MITRE ATT&CK 기반 전술 분류
1. Initial Access (T1190) - 웹 서버 파일 업로드 취약점 악용
2. Execution (T1059) - 웹셸을 통한 원격 명령어 및 스크립트 실행
3. Privilege Escalation (T1068) - WDigest 레지스트리 조작 및 크리덴셜 수집 덫 설치
4. Credential Access (T1003) - Mimikatz를 이용한 LSASS 메모리 자격증명 덤프
5. Lateral Movement (T1021.001) - WinRM / RDP 및 GPO 악용 전사 시스템 장악
6. Impact (T1486) - Cerber 랜섬웨어를 통한 전사 데이터 암호화

##분석 대상 및 가상 인프라 환경
1. 공격 도구: PHP WebShell, WDigest, Fscan, Mimikatz, WMIC, WinRM, Chisel, Cerber Ransomware
2. 구축 환경: VMware Workstation, Active Directory (Windows Server 2019), MS-SQL Server, IIS/XAMPP

## 짱돌 건설 PC 정보 (가상 IP)
웹 서버:	'192.168.0.20' / '192.168.100.20'  (Windows Server 2019)	        
AD 서버:'192.168.100.10'  (Windows Server 2019)	  
DB 서버: '192.168.100.30'  (Windows Server 2019)	   
파일 서버: '192.168.100.40'	 (Windows Server 2019)	   
Executive PC:	'192.168.100.60'	 (Windows 10 Pro)	       
CEO PC:	'192.168.100.25'	 (Windows 10 Pro)	      

## 프로젝트의 산출물
1. 짱돌건설 내부 네트워크 침해사고 분석 보고서 (상세 타임라인 및 디지털 아티팩트 분석 결과)
2.  가상 인프라 구축 가이드라인 및 포렌식 교육용 데이터셋


* 이 프로젝트는 학습용으로 설계되었으며, 다른 목적으로 사용 시 책임을 물을 수 있음. 

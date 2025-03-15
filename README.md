IGLOO Corp, Won Chi Hyun

## 개요
SMB 란 무엇일까? 
SMB란 (Server Message Protocol)로 파일/프린터 공유 프로토콜로 TCP/IP 프로토콜상에서 동작하는 넷바이오스를 통해 네임과 IP 주소가 할당된 컴퓨턷르이 서로 통신할 수 있도록 해준다.    

SMB Broute-force attack => pc의 계정정보 탈취, 시스템 정보 획득 및 파일 변조 시도

테스트 환경

네트워크 스캔 -> nmap ,smb 139, 445가 활성화된 pc 확인

hydra -> administrator 에 대한 smb broute force 공격 실행

희생자 pc 에 대한 시스템 정보 및 팡리 변조
login -> use CS , LS 디렉터리 확인
정상 웹페이지를 웹페이지 변조를 한다.

ESM 에서 Agent 구성 관리- 수집환경 설정

대응방안

포트 비활성화 netbios 137,8,9 ~ smb 139 445 
근거리 통신 망에서 다른 컴퓨터와 공유가 필요없거나 인쇄기 공유가 필요없다면 해당 포트를 닫음으로서 disabled 한다.
장치관리자 - 보기 숨김 장치 표시 - 비 플러그 앤 플레이 드라이버- netbios over tcpip (netbios 닫기)
로컬영역 설정 - 속성 프린터및 파일 공유 해제 (smb 비활성화)

작성자 : Won Chi Hyun
작성일 : 2025.03.15

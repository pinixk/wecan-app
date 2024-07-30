# 위캔필라테스 APP
![info](https://github.com/user-attachments/assets/2a3d7983-01ea-450e-8cb2-4034574421b0)

- 어플리케이션 : [IOS](https://apps.apple.com/kr/app/%EC%9C%84%EC%BA%94%EB%A0%88%EB%94%94/id1609554901) / [Android](https://play.google.com/store/apps/details?id=com.canma.wecan&hl=ko)
- Test ID : 01089773917
- Test PW : 1
 
<br>

## 앱 소개

- 위캔필라테스 회원님들의 간편한 수업 예약 / 취소 기능
- qr코드를 활용한 매장 출입 관리
- 회원님들의 한달 목표 설정 및 운동 / 식단 기록

<br>

### 개발 환경

- Front-end : Flutter
- Back-end : AWS를 활용한 node.js
- 버전 및 이슈관리 : Github, CodePipeline, Elastic Beanstalk
- 협업 툴 : Github, Notion, Slack
- 서비스 배포 환경 : AWS
- DB : MySQL, AWS RDS, S3

<br>

### 마일스톤
- **2023년 2월 - 2023년 4월**
    - 기존 앱 UI 대규모 리뉴얼
    - 여러 핸드폰 기종에 대한 유동적인 UI 개발
    - 다양한 애니메이션 효과 구현

- **2023년 5월 - 2023년 8월**
    - 회원님들 운동 기록 및 식단 기록을 위한 서비스 개발
    - 개인의 목표치를 설정 후 실제 기록을 통한 그래프 구현

- **2023년 9월 - 2023년 10월**
    - 디버깅 작업
    - AWS 활용한 배포

<br>

## 화면구성

### [초기화면]
- 서비스 접속 초기화면으로 splash 화면이 잠시 나온 뒤 초기 페이지
    - 로그인이 되어 있지 않은 경우 : 로그인 페이지
    - 로그인이 되어 있는 경우 : 강사 예약 페이지
| 초기화면 |
|----------|
|![splash](https://github.com/user-attachments/assets/cdb1dac6-0d50-4006-994b-acadb73fa33f)|


### [회원가입]
- 회원권의 타입에 따라 헬스 / 필라테스 구분되어 DB 저장
- 센터를 입력함과 동시에 해당 센터가 표시되어 선택
- 이름 / 비밀번호 / 생년월일 / 휴대폰번호 / 주소 입력
- Naver SMS API를 통한 휴대폰 인증(휴대폰 번호로 로그인 가능하도록 설정되어 있음)
- 도로명주소 API(juso.go.kr)를 통한 주소 검색
| 회원가입 |
|----------|
|![register](https://github.com/user-attachments/assets/50cdb372-d51b-44a7-af0a-75f681d1f15b)|


### [강사예약]
- 달력을 활용한 각 날짜별 강사님 스케일 표시
- 예약 / 대기 / 취소 기능
- 예약자가 한명 빠지면 대기사 1순위 회원님에게 문자 자동 전송
| 강사예약 |
|----------|
|![book](https://github.com/user-attachments/assets/263425f7-df7e-454a-b591-2af68c4c6dba)|


### [QR코드]
- QR코드를 활용한 회원님 출입 서비스 구현
- QR체크 시 회원님의 수업장소 안내
| QR코드 |
|----------|
|![qr](https://github.com/user-attachments/assets/2b35a5f1-1c65-4419-82d2-c155b53c4da6)|


### [회원권]
- 적용되어 있는 회원권 확인
- 회원권 기간 내 예약횟수 / 취소횟수 표시
- 현재 예약 중인 수업 / 대기 중인 수업 / 1:1 PT 현황 표시
| 회원권 |
|----------|
|![ticket](https://github.com/user-attachments/assets/0e8d074a-dcbc-49bf-93ca-0de038078f9d)|


### [일일기록]
- 현재 체중 / 운동 / 식단 / 수면 / 수분 기록
- 이미지 관리는 AWS의 S3로 관리
- 달력을 통한 본인의 일별 기록 열람
| 체중기록 |
|----------|
|![record-weight](https://github.com/user-attachments/assets/9e51c12f-ea32-44d7-b4b2-8d898ca8aa81)|
| 운동기록 |
|----------|
|![record-workout](https://github.com/user-attachments/assets/ffd8f5ca-20e8-4496-ad0c-d43d1cfa4624)|
| 식단기록 |
|----------|
|![record-diet](https://github.com/user-attachments/assets/c8c74cb4-d5dd-415c-a04f-778c3e77d44f)|
| 수면기록 |
|----------|
|![record-sleep](https://github.com/user-attachments/assets/de2811aa-88a1-4269-8073-bc767736af57)|
| 수분기록 |
|----------|
|![record-water](https://github.com/user-attachments/assets/99b6a6fc-f500-4373-9d98-d012485234d2)|
| 달력 |
|----------|
|![record-calendar](https://github.com/user-attachments/assets/77358857-6ada-4901-9a96-a9e04276e2bf)|


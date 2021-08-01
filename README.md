# MQTT-Project-Test-Load-System-Test-Load-Generator
<MQTT 기반 메시지 서버의 성능 모니터링 시스템>의 테스트 로드 시스템 파트입니다.

전체 프로젝트 배경과 설명은 첨부파일-최종 보고서에서 확인 가능합니다.


## 1. 프로젝트 전체 구조
<img src = "https://user-images.githubusercontent.com/38847724/127315703-15176e0d-dbb7-4b4c-a5c6-508073f110a0.png" width="90%" height="90%">


## 2. 그 중 ①Test Load System 파트
<img src = "https://user-images.githubusercontent.com/38847724/127683774-042e2655-2b6c-415d-9a99-d847c3959986.png" width="90%" height="90%">


## 3. 테스트 로드 시스템 구성도
<img src = "https://user-images.githubusercontent.com/38847724/127761039-8c0a1442-0f10-4c14-989f-b1bd9f01d5c9.png" width="80%" height="80%">

 테스트 로드 시스템은 타겟 메시지 서버에 MQTT 메시지를 주고받는 응용을 시뮬레이션 하는 시스템입니다.
 
 - 실제 MQTT 메시지를 유발시키는 여러 대의 client PC들(Raspberry Pi 3 x 10)과, 
 - 이들에게 메시지 유발을 지시하는 master PC, 
 - 그리고 master PC가 client PC들에게 명령을 내리기 위해 사용하는 MQTT Mosquitto Broker(Raspberry Pi 3)와, 
 - Target Message Server로 구성됩니다.
 
 그 중 이곳에는 실제 MQTT 메시지를 유발시키는 여러 대의 client PC들에서 사용하는 Test-Load-Generator 프로그램을 업로드했습니다.

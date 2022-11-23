# 자동차의 최첨단 전자장치와 무선통신을 결합한 스마트카 서비스
### 도메인과 USECASE 이해
- 사물인터넷(IoT)과 빅데이터, 최첨단 전장기술이 결합된 스마트카는 일상에서 타고다니는 자동차 안에 컴퓨터, 무선 인터넷, 전자장치들이 설치되어 자동차 안에서 이메일을 주고받고, 인터넷을 통해 각종 정보도 검색한다. 또한 무선 네트워크를 통해 차량을 원격 진단하고 운전 습관, 날씨, 교통 정보 등을 분석해서 운전자의 안전과 편의를 도모한다. 국내외 주요 IT기업들(구글, 애플, 삼성 등)이 최첨단 기술을 이용해 스마트카 산업을 주도하기 시작했으며 무인 자동차의 테스트베드 성공이 가시화 되고 있다.
- 스마트카 안에는 수백 개의 IoT 센서가 장착되어 있으며, 자동차의 상태를 모니터링 하면서 수많은 차량 상태 정보를 실시간으로 만들어낸다. 스마트카의 센싱 정보는 무선 네트워크를 타고 중앙의 빅데이터 시스템으로 전송되며, 이 데이터들은 수집->적재->처리 및 탐색->분석 및 응용 단계를 거치면서 운전자에게 편의성과 안전성을 지원하는 스마트카 서비스로 제공된다. 이러한 스마트카에서 발생하는 수많은 데이터로부터 가치와 통찰력을 찾기 위한 빅데이터 시스템을 파일럿 프로젝트로 진행하고자 한다.
--------
### 요구사항 파악
- 요구사항1 : 차량의 다양한 장치로부터 발생하는 로그 파일을 수집해서 기능별 상태를 점검한다.
- 요구사항2 : 운전자의 운행 정보가 담긴 로그를 실시간으로 수집해서 주행 패턴을 분석한다.
### 기본 데이터셋 
1. 스마트카 상태 정보 데이터셋 : 스마트카의 각종 센서로부터 발생하는 차량의 상태 정보 데이터셋으로 요구사항1과 직접적인 관련이 있으며, 로그 시뮬레이터를 통해 생성된다.
2. 스마트카 운전자 운행 데이터셋 : 스마트카 운전자의 운전패턴/운행정보가 담긴 데이터셋으로 요구사항2와 직접적인 관련이 있으며, 로그 시뮬레이터를 통해 생성된다.
3. 스마트카 마스터 데이터셋 : 스마트카 운전자의 프로파일 정보가 담긴 데이터셋으로, 요구사항1,2와 관련된 분석 데이터셋을 만들 때 활용한다. (이미 만들어진 샘플 파일 이용)
4. 스마트카 물품구매 이력 데이터셋 : 스마트카 운전자가 차량 내의 스마트 스크린을 통해 쇼핑몰에서 구입한 차량 물품 구매 목록 데이터셋으로 요구사항 1,2와 관련된 분석 데이터셋을 만들 때 활용한다. (이미 만들어진 샘플 파일 이용)
*소규모 빅데이터 파일럿 환경을 구성 : 가상 머신 3대를 만들어 빅데이터 분산 환경을 만들고 필요한 빅데이터 컴포넌트들을 추가 및 확장한다. 

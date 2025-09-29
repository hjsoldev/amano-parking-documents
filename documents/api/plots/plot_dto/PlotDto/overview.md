# Overview for `PlotDto`

## Description

# 주차장 목록 요청(지도 범위 기반 조회)

 - GET /plots

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |minLatitude|double|최소 위도|
  |minLongitude|double|최소 경도|
  |maxLatitude|double|최대 위도|
  |maxLongitude|double|최대 경도|
  |plotTicketType|string|주차권 타입 (주차권, 정기권) 공란시 전체 조회|
  |plotTicketTime|string|주차권 시간, 공란시 전체 조회|
  |plotTicketPeriod|string|주차권 기간 (평일오전, 평일오후, 주말오전, 주말오후, 종일권) 공란시 전체 조회|

 - plotTicketTime - 필터에 사용되는 주차권 시간 - 숫자, 공란시 전체 조회
 - plotTicketPeriod - 필터에 사용되는 주차권 기간 - 확인 후 삭제?

 - 요청 파라미터 예시

 ```json
 {
   "minLatitude": 37.480694,
   "minLongitude": 126.882096,
   "maxLatitude": 37.480694,
   "maxLongitude": 126.882096
   "plotTicketType": "regular",
   "plotTicketTime": "1",
   "plotTicketPeriod": "all",
 }
 ```

 - plotTicketType값
   - regular: 주차권
   - season: 정기권
 - plotTicketPeriod값
   - all: 전체
   - weekdayMorning: 평일오전
   - weekdayAfternoon: 평일오후
   - weekendMorning: 주말오전
   - weekendAfternoon: 주말오후
   - allDay: 종일권

 # 주차장 목록 요청(줌 레벨 기반 조회) - 현재 미사용

 - GET /plots/zoom

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |latitude|double|위도|
  |longitude|double|경도|
  |zoomLevel|double|줌 레벨|

 - 요청 파라미터 예시

 ```json
 {
   "latitude": 37.480694,
   "longitude": 126.882096,
   "zoomLevel": 10
 }
 ```

 # 주차장 검색

 - GET /plots/keyword

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |keyword|string|검색 키워드|

 - 요청 파라미터 예시

 ```json
 {
   "keyword": "주차장"
 }
 ```

 # 주차장 목록 응답

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |contents|arr_PlotInfoDto|주차장 목록|

 - 응답 파라미터 예시

 ```json
 [
   {
     "plotId": "00001",
     "plotNam": "주차장 이름",
     "addr": "주차장 주소",
     "lngt": 127.111128,
     "ltd": 37.394981,
     "plotTicketType": "regular",
     "plotTicketTime": "",
     "plotStatus": ["available"],
     "plotOp": {
       "dtlGid": "정기권 차량은 입구에서 별도의 정기권 인증 절차를 진행한 뒤 주차장에 진입해 주십시오.",
     },
     "pfOp": {
       "bildNm": "건물명",
       "bildForms": ["public"],
       "plotForms": ["machine", "auto"],
       "usePsblCarKinds": ["suv", "sedan"],
       "totPakCnt": 123,
     },
     "ppOp": {
       "name": "1시간권",
       "price": 2000,
       "discount": 50,
       "status": "sale",
       "description": "1시간권",
     }
   },
   {
     "plotId": "00002",
     "plotNm": "주차장 이름",
     "addr": "주차장 주소",
     "plotClasGrpCd": "주차장 종류",
     "lngt": 127.120981,
     "ltd": 37.387216,
     "plotTicketType": "regular",
     "plotTicketTime": "",
     "plotStatus": ["available"],
     "plotOp": {
       "dtlGid": "정기권 차량은 입구에서 별도의 정기권 인증 절차를 진행한 뒤 주차장에 진입해 주십시오.",
     },
     "pfOp": {
       "bildNm": "건물명",
       "bildForms": ["public"],
       "plotForms": ["machine", "auto"],
       "totPakCnt": 123,
     },
     "ppOp": {
       "name": "2시간권",
       "price": 3000,
       "discount": 20,
       "status": "sale",
       "description": "1시간권",
     }
   },
   {
     "plotId": "00003",
     "plotNm": "주차장 이름3",
     "addr": "주차장 주소3",
     "plotClasGrpCd": "주차장 종류",
     "lngt": 127.130981,
     "ltd": 37.377216,
     "plotTicketType": "regular",
     "plotTicketTime": "",
     "plotStatus": ["coupon"],
     "plotOp": {
       "dtlGid": "정기권 차량은 입구에서 별도의 정기권 인증 절차를 진행한 뒤 주차장에 진입해 주십시오.",
     },
     "pfOp": {
       "bildNm": "건물명",
       "bildForms": ["public"],
       "plotForms": ["machine", "auto"],
       "totPakCnt": 123,
     },
     "ppOp": {
       "name": "3시간권",
       "price": 4000,
       "discount": 30,
       "status": "sale",
       "description": "3시간권",
     }
   },
 ]
 ```

 # 주차장 정보

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|string|주차장 ID|
  |plotNm|string|주차장 이름|
  |addr|string|주차장 주소|
  |lngt|double|경도|
  |ltd|double|위도|
  |plotTicketType|string?|주차장 타입(주차권, 정기권)|
  |plotTicketTime|string?|주차권 시간(숫자만)|
  |plotStatus|string?|주차장 상태(이용불가, 할인 이벤트, 쿠폰)|
  |plotOp|PlotOperationDto?|주차장 운영 정보|
  |pfOp|PlotFacilityOperationDto?|주차장 시설 정보|
  |ppOp|PlotProductOperationDto?|주차장 상품 정보|

 - plotTicketType 값
    - regular:주차권
    - season:정기권
 - plotStatus 값 - 지도 마커의 상태 표시
    - none:상태없음
    - unavailable:이용불가
    - discount:할인 이벤트
    - coupon:쿠폰

## Dependencies

- _$PlotDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

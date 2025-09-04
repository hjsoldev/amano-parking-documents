# Overview for `PlotDto`

## Description

# 주차장 목록 요청(지도 범위 기반 조회)

 - POST /plots

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |minLatitude|double|최소 위도|
  |minLongitude|double|최소 경도|
  |maxLatitude|double|최대 위도|
  |maxLongitude|double|최대 경도|
  |plotTicketType|string|주차권 타입 (주차권, 정기권) 공란시 전체 조회|
  |plotTicketTime|string|주차권 시간 (1시간, 2시간, 3시간, 4시간, 5시간, 6시간, 12시간) 공란시 전체 조회|
  |plotTicketPeriod|string|주차권 기간 (평일오전, 평일오후, 주말오전, 주말오후, 종일권) 공란시 전체 조회|

 - 요청 파라미터 예시

 ```json
 {
   "minLatitude": 37.480694,
   "minLongitude": 126.882096,
   "maxLatitude": 37.480694,
   "maxLongitude": 126.882096
   "plotTicketType": "regular",
   "plotTicketTime": "all",
   "plotTicketPeriod": "all",
 }
 ```

 - plotTicketType값
   - regular: 주차권
   - season: 정기권
 - plotTicketTime값
   - all: 전체
   - onehour: 1시간
   - twohour: 2시간
   - threehour: 3시간
   - fourhour: 4시간
   - fivehour: 5시간
   - sixhour: 6시간
   - twelvehour: 12시간
 - plotTicketPeriod값
   - all: 전체
   - weekdayMorning: 평일오전
   - weekdayAfternoon: 평일오후
   - weekendMorning: 주말오전
   - weekendAfternoon: 주말오후
   - allDay: 종일권

 # 주차장 목록 요청(줌 레벨 기반 조회)

 - POST /plots/zoom

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

 - POST /plots/keyword

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
  |plots|List<PlotInfoDto>|주차장 목록|
  |meta|MetaDto|메타 데이타|

 - 응답 파라미터 예시
 ```json
 {
   "plots": [
     {
       "plotId": "00001",
       "plotNm": "주차장 이름",
       "addr": "주차장 주소",
       "plotClasGrpCd": "주차장 종류",
       "lngt": 127.111128,
       "ltd": 37.394981,
       "plotTicketName": "주차권 이름",
       "plotTicketType": "regular",
       "plotTicketPrice": 1000,
       "plotStatus": ["available"],
       "plotTagList": ["lift", "electric"]
     },
     {
       "plotId": "00002",
       "plotNm": "주차장 이름",
       "addr": "주차장 주소",
       "plotClasGrpCd": "주차장 종류",
       "lngt": 127.120981,
       "ltd": 37.387216,
       "plotTicketName": "주차권 이름",
       "plotTicketType": "regular",
       "plotTicketPrice": 1000,
       "plotStatus": ["available"],
       "plotTagList": ["machine", "auto"]
     },
   ],
   "meta": {
     "totalItems": 2,
     "itemCount": 2,
     "itemsPerPage": 1,
     "totalPages": 1,
     "currentPage": 1
   }
 }
 ```

 - plotTagList값
   - none: 일반
   - machine: 기계식
   - auto: 자주식
   - lift: 리프트
   - ground: 노상
   - mixed: 복합
   - sub: 부설주
   - electric: 전기차 충전

## Dependencies

- _$PlotDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
### fromResponse


#### Parameters

- `response`: `dynamic`

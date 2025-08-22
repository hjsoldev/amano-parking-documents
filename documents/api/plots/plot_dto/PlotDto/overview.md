# Overview for `PlotDto`

## Description

# 주차장 목록 요청(지도 범위 기반 조회)

 - POST /api/plots

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |minLatitude|double|최소 위도|
  |minLongitude|double|최소 경도|
  |maxLatitude|double|최대 위도|
  |maxLongitude|double|최대 경도|

 - 요청 파라미터 예시

 ```json
 {
   "minLatitude": 37.480694,
   "minLongitude": 126.882096,
   "maxLatitude": 37.480694,
   "maxLongitude": 126.882096
 }
 ```

 # 주차장 목록 요청(줌 레벨 기반 조회)

 - POST /api/plots/zoom

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

 - POST /api/plots/keyword

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
       "ltd": 37.394981
     },
     {
       "plotId": "00002",
       "plotNm": "주차장 이름",
       "addr": "주차장 주소",
       "plotClasGrpCd": "주차장 종류",
       "lngt": 127.120981,
       "ltd": 37.387216
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

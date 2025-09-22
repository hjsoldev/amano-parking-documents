# Overview for `PlotDetailDto`

## Description

# 주차장 상세 정보 요청

 - GET /plots/{plotId}

 # 주차장 상세 정보 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |plotId|string|주차장 고유 아이디|
 |plotNm|string|주차장 이름|
 |addr|string|주차장 주소|
 |lngt|double|주차장 경도|
 |ltd|double|주차장 위도|
 |plotOp|PlotOperationDto?|주차장 운영 정보|
 |pfOp|PlotFacilityOperationDto?|주차장 시설 운영 정보|
 |ppOp|arr_PlotProductOperationDto?|주차장 상품 운영 정보|
 |plotLastUpdated|string?|주차장 정보 마지막 업데이트 시간|

 - 응답 데이터 예시

 ```json

 {
   "plotId": "1234567890",
   "plotNm": "주차장 이름",
   "addr": "주차장 주소",
   "lngt": 127.111128,
   "ltd": 37.394981,
   "plotOp": PlotOperationDto,
   "pfOp": PlotFacilityOperationDto,
   "ppOp": [PlotProductOperationDto, PlotProductOperationDto],
   "plotLastUpdated": "2025-01-01",
 }
 ```

## Dependencies

- _$PlotDetailDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
### fromResponse


#### Parameters

- `response`: `dynamic`

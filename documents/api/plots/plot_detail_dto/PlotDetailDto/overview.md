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
 |plotClasGrpCd|string|주차장 클래스 그룹 코드|
 |lngt|double|주차장 경도|
 |ltd|double|주차장 위도|
 |plotOp|object|주차장 운영 정보|
 |pfOp|object|주차장 시설 운영 정보|

 - 응답 데이터 예시

 ```json

 {
   "plotId": "1234567890",
   "plotNm": "주차장 이름",
   "addr": "주차장 주소",
   "plotClasGrpCd": "PAK_CLAS_GE",
   "lngt": 127.111128,
   "ltd": 37.394981,
   "plotOp": PlotOperationDto,
   "pfOp": PlotFacilityOperationDto,
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

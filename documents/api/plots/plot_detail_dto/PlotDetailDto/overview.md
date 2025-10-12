# Overview for `PlotDetailDto`

## Description

# 주차장 정보

  |이름|타입|설명|
  |-|-|-|
  |plotId|string|주차장 ID|
  |plotNm|string|주차장 이름|
  |addr|string|주차장 주소|
  |lngt|double|경도|
  |ltd|double|위도|
  |plotOp|PlotOperationDto?|주차장 운영 정보|
  |pfOp|PlotFacilityOperationDto?|주차장 시설 정보|
  |ppOp|arr_PlotProductOperationDto?|주차장 상품 정보|
  |plotLastUpdated|string?|주차장 마지막 업데이트 시간|

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

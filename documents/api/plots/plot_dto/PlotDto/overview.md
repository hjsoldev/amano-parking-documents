# Overview for `PlotDto`

## Description

# 주차장 정보

  |이름|타입|설명|
  |-|-|-|
  |plotId|string|주차장 ID|
  |plotNm|string|주차장 이름|
  |addr|string|주차장 주소|
  |lngt|double|경도|
  |ltd|double|위도|
  |plotTicketType|string?|주차장 타입(주차권, 정기권)|
  |plotStatus|string?|주차장 상태(이용불가, 할인 이벤트, 쿠폰)|
  |plotOp|PlotOperationDto?|주차장 운영 정보|
  |pfOp|PlotFacilityOperationDto?|주차장 시설 정보|
  |ppOp|PlotProductOperationDto?|주차장 상품 정보|

## Dependencies

- _$PlotDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
### fromResponse


#### Parameters

- `content`: `Object?`

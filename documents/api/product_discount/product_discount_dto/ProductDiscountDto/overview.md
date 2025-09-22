# Overview for `ProductDiscountDto`

## Description

# 상품 할인 정보 요청

 - GET /product-discounts

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |minLatitude|double|최소 위도|
  |maxLatitude|double|최대 위도|
  |minLongitude|double|최소 경도|
  |maxLongitude|double|최대 경도|

 - 요청 파라미터 예시

 ```json
 {
   "minLatitude": 37.480694,
   "maxLatitude": 37.480694,
   "minLongitude": 126.882096,
   "maxLongitude": 126.882096
 }
 ```

 # 상품 할인 정보 응답

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotInfo|PlotInfoDto|주차장 정보|
  |plotOp|PlotOperationDto|주차장 운영 정보|
  |pfOp|PlotFacilityOperationDto|주차장 시설 정보|
  |ppOp|PlotProductOperationDto|주차장 상품 정보|
  |distance|double|거리(미터)|

 - 응답 파라미터 예시

 ```json
 {
   "plotInfo": PlotInfoDto,
   "plotOp": PlotOperationDto,
   "pfOp": PlotFacilityOperationDto,
   "ppOp": PlotProductOperationDto,
   "distance": 123.456
 }
 ```

## Dependencies

- _$ProductDiscountDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

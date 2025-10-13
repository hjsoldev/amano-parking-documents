# Method: `getProductDiscount`

## Description

# 상품 할인 정보 요청

 ## GET /product-discounts

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |minLatitude|double|최소 위도|
  |maxLatitude|double|최대 위도|
  |minLongitude|double|최소 경도|
  |maxLongitude|double|최대 경도|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotInfo|PlotDto|주차장 정보|

 ### 거리 항목은 로컬에서 계산?

## Return Type
`Future<Either<AppException, WrapperDto<ProductDiscountDto>>>`

## Parameters

- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`

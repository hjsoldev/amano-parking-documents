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

  ### 응답 파라미터 설명

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

 ### 거리 항목은 로컬에서 계산?

## Return Type
`Future<Either<AppException, WrapperDto<ProductDiscountDto>>>`

## Parameters

- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`

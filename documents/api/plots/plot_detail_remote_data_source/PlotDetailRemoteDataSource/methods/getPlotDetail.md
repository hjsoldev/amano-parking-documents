# Method: `getPlotDetail`

## Description

# 주차장 상세 정보 요청

 ## GET /plots/{plotId}

 ### 응답 파라미터 설명

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

## Return Type
`Future<Either<AppException, WrapperDto<PlotDetailDto>>>`

## Parameters

- ``: `dynamic`

# Method: `getFavorites`

## Description

# 즐겨찾기 목록 요청

 ## GET /favorites

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

 ### 확인 필요 사항
 - pfOp의 bildForms 필드의 값중 amano가 있으면 아마노 주차장 아이콘을 표시 중입니다.

## Return Type
`Future<Either<AppException, WrapperDto<PlotDto>>>`


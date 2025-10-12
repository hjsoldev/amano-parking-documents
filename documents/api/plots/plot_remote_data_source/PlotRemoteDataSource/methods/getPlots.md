# Method: `getPlots`

## Description

# 주차장 목록 요청(지도 범위 기반 조회)

 ## GET /plots

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |minLatitude|double|최소 위도|
  |minLongitude|double|최소 경도|
  |maxLatitude|double|최대 위도|
  |maxLongitude|double|최대 경도|
  |plotTicketType|string|주차권 타입 (주차권, 정기권) 공란시 전체 조회|
  |plotTicketTime|string|주차권 시간, 공란시 전체 조회|
  |plotTicketPeriod|string|주차권 기간 (평일오전, 평일오후, 주말오전, 주말오후, 종일권) 공란시 전체 조회|

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

 ### plotTicketType

 - regular: 주차권
 - season: 정기권

 ### plotTicketTime

 - 필터에 사용되는 주차권 시간 - 숫자, 공란시 전체 조회

 ### plotTicketPeriod

 - 필터에 사용되는 주차권 기간 - 확인 후 삭제?

 ### 확인 필요 사항

 - 필터 관련 내용 수정 필요

## Return Type
`Future<Either<AppException, WrapperDto<PlotDto>>>`

## Parameters

- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`

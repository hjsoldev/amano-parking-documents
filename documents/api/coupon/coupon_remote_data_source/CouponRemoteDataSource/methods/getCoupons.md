# Method: `getCoupons`

## Description

# 쿠폰 목록 요청

 ## GET /coupon

 ### 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |status|string|쿠폰 상태|

 ### status
 - available: 사용 가능
 - expired: 만료

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|쿠폰 아이디|
 |title|string|쿠폰 제목|
 |description|string|쿠폰 설명|
 |startDate|string|쿠폰 시작 날짜|
 |endDate|string|쿠폰 종료 날짜|
 |plotName|string|주차장 이름|
 |status|string|쿠폰 상태|
 |linkType|string|이동 경로|
 |linkId|string|주차장 상세페이지 아이디|

 ### status
 - available: 사용 가능
 - expired: 만료
 - used: 사용 완료
 - closed: 중단

 ### linkType
 - plot: 주차장

## Return Type
`Future<Either<AppException, WrapperDto<CouponDto>>>`

## Parameters

- `type`: `String`

# Method: `getSubscriptions`

## Description

# 구독 내역 요청

 ## GET /subscriptions/{type}

 ### 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |type|string|타입|

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|아이디|
 |plotName|string|주차장 이름|
 |carNumber|string|차량 번호|
 |reservationDate|string|다음 결제 예약 날자|
 |reservationCard|string|다음 결제 예약 카드|
 |amount|int|금액|
 |status|string|상태|
 |type|string|타입|
 |latitude|double|위도|
 |longitude|double|경도|

 ### type 값
 - available: 구독 현황
 - expired: 만료된 구독

 ### status 값
 - using: 사용중
 - wait: 사용대기
 - complete: 사용완료
 - expired: 기간만료
 - cancel: 결제취소

## Return Type
`Future<Either<AppException, WrapperDto<SubscriptionDto>>>`

## Parameters

- `type`: `String`

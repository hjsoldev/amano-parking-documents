# Method: `getHistory`

## Description

# 주차권 사용 내역 요청

 ## GET /history/uses

 ### 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |beginDate|string|시작 날짜|
 |endDate|string|종료 날짜|

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|사용 ID|
 |plotId|string|주차장 ID|
 |plotName|string|주차장 이름|
 |plotAddress|string|주차장 주소|
 |ticketId|string|주차권 ID|
 |ticketdName|string|주차권 이름(상품명)|
 |carNumber|string|차량번호|
 |isSubscribed|bool|구독 상품 여부|
 |discount|map_(string, string)|할인 내용|
 |totalAmount|int|총 주차 요금|
 |inTime|string|입차 시간|
 |passedTime|string|주차 시간|
 |estimateAmount|int|정산 예상 금액|
 |status|string|구매 상태 (예: 완료, 취소, 환불 등)|

 ### status
 - wait: 대기
 - using: 사용중
 - expired: 만료
 - cancel: 취소
 - complete: 완료

## Return Type
`Future<Either<AppException, WrapperDto<HistoryUseDto>>>`

## Parameters

- ``: `dynamic`
- ``: `dynamic`

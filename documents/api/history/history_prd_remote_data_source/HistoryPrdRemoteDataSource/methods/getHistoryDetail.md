# Method: `getHistoryDetail`

## Description

# 상품 내역 상세 요청

 ## GET /history/products/{id}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|상품 ID|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|상품 ID|
  |plotId|string|주차장 ID|
  |ticketId|string|주차권 ID|
  |prodName|string|상품명|
  |plotName|string|지점명|
  |plotAddress|string|지점 주소|
  |carNumber|string|차량번호|
  |isSubscribed|bool|구독 상품 여부|
  |discount|map_(string, string)|할인 내용|
  |price|int|상품 단가|
  |startDate|string|상품 유효 기간 시작일|
  |endDate|string|상품 유효 기간 만료일|
  |purchaseDate|string|구매 일시|
  |status|string|구매 상태 (예: 완료, 취소, 환불 등)|
  |remainCount|int|남은 차량 변경 횟수|

 ### status
 - wait: 대기
 - using: 사용중
 - expired: 만료
 - cancel: 취소
 - complete: 완료

## Return Type
`Future<Either<AppException, WrapperDto<HistoryPrdDto>>>`

## Parameters

- ``: `dynamic`

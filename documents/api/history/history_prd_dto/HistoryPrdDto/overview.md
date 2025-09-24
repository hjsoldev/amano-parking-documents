# Overview for `HistoryPrdDto`

## Description

# 주차권 구매 내역 요청

 - GET /history/products

 - 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |beginDate|string|시작 날짜|
 |endDate|string|종료 날짜|

 - 요청 파라미터 예시

 ```json
 {
   "beginDate": "2025-08-21",
   "endDate": "2025-08-22"
 }
 ```

 # 주차권 구매 내역 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|상품 ID|
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

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "123e4567-e89b-12d3-a456-426614174000",
     "prodName": "1시간권",
     "plotName": "이마트 성수점",
     "plotAddress": "서울특별시 성동구 왕십리로 100",
     "carNumber": "789다1234",
     "isSubscribed": false,
     "discount": [{"쿠폰": "10%"}, {"포인트": "1000원"}],
     "price": 15000,
     "startDate": "2025-08-21",
     "endDate": "2025-08-22",
     "purchaseDate": "2025-08-21T03:45:30.123456Z",
     "status": "complete"
   }
   {
     "id": "123e4567-e89b-12d3-a456-426614174001",
     "prodName": "1시간권",
     "plotName": "이마트 성수점",
     "plotAddress": "서울특별시 성동구 왕십리로 100",
     "carNumber": "789다1234",
     "isSubscribed": false,
     "discount": [{"쿠폰": "10%"}, {"포인트": "1000원"}],
     "price": 15000,
     "startDate": "2025-08-21",
     "endDate": "2025-08-22",
     "purchaseDate": "2025-08-21T03:45:30.123456Z",
     "status": "wait"
   }
 ]
 ```

 - status 값
   - wait: 대기
   - using: 사용중
   - expired: 만료
   - cancel: 취소
   - complete: 완료

## Dependencies

- _$HistoryPrdDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

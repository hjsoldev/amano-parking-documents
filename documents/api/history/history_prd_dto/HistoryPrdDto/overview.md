# Overview for `HistoryPrdDto`

## Description

# 주차권 구매 내역

 - POST /history/products

 # 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |beginDate|String|시작 날짜(ISO 8601 형식)|
 |endDate|String|종료 날짜(ISO 8601 형식)|

 # 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|String|상품 ID|
 |productName|String|상품명|
 |stationName|String|지점명|
 |carNumber|String|차량번호|
 |isSubscribed|bool|구독 상품 여부|
 |discount|List<(String, String)>|할인 내용|
 |price|String|상품 단가|
 |startDate|String|상품 유효 기간 시작일|
 |endDate|String|상품 유효 기간 만료일|
 |purchaseDate|String|구매 일시|
 |status|String|구매 상태 (예: 완료, 취소, 환불 등)|

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

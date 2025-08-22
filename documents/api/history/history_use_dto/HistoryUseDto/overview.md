# Overview for `HistoryUseDto`

## Description

# 주차권 사용 내역 요청

 - POST /history/uses

 - 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |beginDate|String|시작 날짜(ISO 8601 형식)|
 |endDate|String|종료 날짜(ISO 8601 형식)|

 - 요청 파라미터 예시

 ```json
 {
   "beginDate": "2025-08-21",
   "endDate": "2025-08-22"
 }
 ```

 # 주차권 사용 내역 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|String|사용 ID|
 |productName|String|상품명|
 |stationName|String|지점명|
 |carNumber|String|차량번호|
 |isSubscribed|bool|구독 상품 여부|
 |discount|List<(String, String)>|할인 내용|
 |totalAmount|String|총 주차 요금|
 |inTime|String|입차 시간|
 |passedTime|String|주차 시간|
 |estimateAmount|String|정산 예상 금액|
 |status|String|구매 상태 (예: 완료, 취소, 환불 등)|

 - status 값
   - wait: 대기
   - using: 사용중
   - expired: 만료
   - cancel: 취소
   - complete: 완료

## Dependencies

- _$HistoryUseDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

# Overview for `CouponDto`

## Description

# 쿠폰 목록 요청

 ## 쿠폰 사용 가능 목록 요청
 - GET /api/coupon/available

 ## 쿠폰 만료 목록 요청
 - GET /api/coupon/expired

 # 쿠폰 목록 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|쿠폰 ID|
 |title|string|쿠폰 제목|
 |amount|int|쿠폰 금액|
 |description|string|쿠폰 설명|
 |startDate|string|쿠폰 시작 날짜|
 |endDate|string|쿠폰 종료 날짜|
 |status|string|쿠폰 상태|
 |type|string|쿠폰 타입|
 |parkingLotName|string|쿠폰 주차장 이름|
 |minimumAmount|int|쿠폰 최소 금액|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "123e4567-e89b-12d3-a456-426614174000",
     "title": "쿠폰1",
     "amount": 10000,
     "description": "쿠폰 설명",
     "startDate": "2025-08-20T10:00:00Z",
     "endDate": "2025-08-20T10:00:00Z",
     "status": "available",
     "type": "discount",
     "parkingLotName": "주차장 이름",
     "minimumAmount": 10000
   },
   {
     "id": "123e4567-e89b-12d3-a456-426614174000",
     "title": "쿠폰2",
     "amount": 10000,
     "description": "쿠폰 설명",
     "startDate": "2025-08-20T10:00:00Z",
     "endDate": "2025-08-20T10:00:00Z",
     "status": "expired",
     "type": "discount",
     "parkingLotName": "주차장 이름",
     "minimumAmount": 10000
   }
 ]
 ```

## Dependencies

- _$CouponDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

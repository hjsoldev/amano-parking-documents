# Overview for `CouponDto`

## Description

# 쿠폰 목록 요청

 ## 쿠폰 사용 가능 목록 요청

 - GET /coupon

 - 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |status|string|쿠폰 상태|

 - status 값
   - available: 사용 가능
   - expired: 만료

 # 쿠폰 목록 응답

 - 응답 파라미터 설명

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

 - status 값
   - available: 사용 가능
   - expired: 만료
   - used: 사용 완료
   - closed: 중단

 - linkType
   - plot: 주차장

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "쿠폰1",
     "plotName": "주차장 이름1",
     "description": "쿠폰 설명1",
     "startDate": "2025-08-20T10:00:00Z",
     "endDate": "2025-08-20T10:00:00Z",
     "status": "available",
     "linkType": "plot",
     "linkId": "1",
   },
   {
     "id": "2",
     "title": "쿠폰2",
     "plotName": "주차장 이름2",
     "description": "쿠폰 설명2",
     "startDate": "2025-08-20T10:00:00Z",
     "endDate": "2025-08-20T10:00:00Z",
     "status": "available",
     "linkType": "plot",
     "linkId": "2",
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

# Overview for `CouponRegistrationDto`

## Description

# 쿠폰 등록 요청

 - POST /coupons/register

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |couponCode|string|쿠폰 코드|

 - 요청 파라미터 예시

 ```json
 {
   "couponCode": "1234567890"
 }
 ```

 # 쿠폰 등록 응답

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |isSuccess|boolean|성공 여부|
  |message|string|메시지|
  |couponId|string|쿠폰 ID|
  |couponTitle|string|쿠폰 제목|
  |couponDescription|string|쿠폰 설명|

 - 응답 파라미터 예시

 ```json
 {
   "isSuccess": true,
   "message": "쿠폰 등록 요청이 완료되었습니다.",
   "couponId": "123e4567-e89b-12d3-a456-426614174000",
   "couponTitle": "쿠폰1",
   "couponDescription": "쿠폰 설명"
 }
 ```

## Dependencies

- _$CouponRegistrationDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

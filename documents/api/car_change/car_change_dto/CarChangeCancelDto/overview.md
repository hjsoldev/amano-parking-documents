# Overview for `CarChangeCancelDto`

## Description

# 치량 변경 취소 요청

 - POST /api/car-change/cancel

 - 요청 데이터 설명

 |이름|타입|설명|
 |-|-|-|
 |requestId|string|차량 변경 요청 ID|

 - 요청 데이터 예시

 ```json
 {
   "requestId": "123e4567-e89b-12d3-a456-426614174000"
 }
 ```

 # 차량 변경 취소 응답

 - 응답 데이터 설명

 |이름|타입|설명|
 |-|-|-|
 |success|boolean|성공 여부|
 |message|string|메시지|

 - 응답 데이터 예시

 ```json
 {
   "success": true,
   "message": "차량 변경 취소 요청이 완료되었습니다."
 }
 ```

## Dependencies

- _$CarChangeCancelDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
### fromResponse


#### Parameters

- `response`: `dynamic`
### empty



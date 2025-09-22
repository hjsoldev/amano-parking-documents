# Overview for `CarChangeDto`

## Description

# 차량 변경 요청

 - PUT /car-change/submit

 - 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |currentCarNumber|string|현재 차량 번호|
 |newCarNumber|string|변경할 차량 번호|
 |changeDate|string|변경할 날짜 (YYYY-MM-DD)|

 - 요청 파라미터 예시

 ```json
 {
   "currentCarNumber": "123가1234",
   "newCarNumber": "456가4567",
   "changeDate": "2025-08-21"
 }
 ```

 # 차량 변경 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|차량 변경 요청 ID|
 |remainCount|int|남은 차량 변경 횟수|

 - 응답 파라미터 예시

 ```json
 {
   "id": "123e4567-e89b-12d3-a456-426614174000",
   "remainCount": 3
 }
 ```

## Dependencies

- _$CarChangeDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
### fromResponse


#### Parameters

- `response`: `dynamic`
### empty



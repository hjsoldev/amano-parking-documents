# Overview for `NotificationDto`

## Description

# 알림(시스템, 이벤트) 목록 요청

 - GET /notification/{type}

 - 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |type|string|알림 타입(시스템, 이벤트)|

 - type 값
   - system: 시스템
   - event: 이벤트

 # 알림(시스템, 이벤트) 목록 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|알림 ID|
 |type|string|알림 타입(시스템, 이벤트)|
 |carNumber|string|차량번호|
 |title|string|타이틀|
 |bodyMsg|string|메시지|
 |footMsg|string|하단 메시지|
 |linkType|string|이동 경로(event, notice ... etc)|
 |linkId|string|이동 경로 아이디|
 |createAt|string|날짜|

 - 응답 파라미터 예시

 ```json
 {
   "id": "1",
   "type": "system",
   "carNumber": "123가1234",
   "title": "타이틀",
   "bodyMsg": "메시지",
   "footMsg": "하단 메시지",
   "linkType": "event",
   "linkId": "1",
   "createAt": "2024-01-15"
 }
 ```

 - linkType 값
   - event: 이벤트
   - notice: 공지사항
   - coupon: 쿠폰
   - system: 시스템

## Dependencies

- _$NotificationDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

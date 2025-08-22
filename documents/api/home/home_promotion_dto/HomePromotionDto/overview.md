# Overview for `HomePromotionDto`

## Description

# 홈 화면에서 보여지는 프로모션(배너) 데이터 요청

 - GET /home/promotion

 # 홈 화면에서 보여지는 프로모션(배너) 데이터 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|프로모션 고유 아이디|
 |title|string|프로모션 타이틀|
 |type|string|프로모션 타입|
 |message|string|프로모션 메시지|
 |imageUrl|string|프로모션 이미지 URL|
 |startAt|string|프로모션 시작일|
 |endAt|string|프로모션 종료일|
 |createAt|string|프로모션 생성 날짜|
 |status|string|프로모션 상태(?)|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "프로모션 타이틀",
     "type": "promotion",
     "message": "프로모션 메시지",
     "imageUrl": "https://example.com/image.png",
     "startAt": "2025-08-20T10:00:00Z",
     "endAt": "2025-08-20T10:00:00Z",
     "createAt": "2025-08-20T10:00:00Z",
     "status": "active"
   },
   {
     "id": "2",
     "title": "프로모션 타이틀2",
     "type": "promotion",
     "message": "프로모션 메시지2",
     "imageUrl": "https://example.com/image.png",
     "startAt": "2025-08-20T10:00:00Z",
     "endAt": "2025-08-20T10:00:00Z",
     "createAt": "2025-08-20T10:00:00Z",
     "status": "active"
   }
 ]
 ```

## Dependencies

- _$HomePromotionDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

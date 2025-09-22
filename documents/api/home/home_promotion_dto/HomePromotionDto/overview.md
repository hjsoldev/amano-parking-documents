# Overview for `HomePromotionDto`

## Description

# 홈 화면에서 보여지는 프로모션(배너) 데이터 요청

 - GET /home/banner/M02

 # 홈 화면에서 보여지는 프로모션(배너) 데이터 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|배너(프로모션) 고유 아이디|
 |title|string|배너(프로모션) 타이틀|
 |subTitle|string|배너(프로모션) 서브타이틀|
 |imageUrl|string|배너(프로모션) 이미지 URL|
 |contentType|string|배너(프로모션) 컨텐츠 타입|
 |contentId|string|배너(프로모션) 컨텐츠 아이디|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "배너(프로모션) 타이틀",
     "subTitle": "프로모션 서브타이틀",
     "imageUrl": "https://example.com/image.png",
     "contentType": "promotion",
     "contentId": "1",
   },
   {
     "id": "2",
     "title": "배너(프로모션) 타이틀2",
     "subTitle": "프로모션 서브타이틀2",
     "imageUrl": "https://example.com/image.png",
     "contentType": "promotion",
     "contentId": "2",
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

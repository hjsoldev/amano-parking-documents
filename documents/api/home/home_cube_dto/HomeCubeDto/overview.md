# Overview for `HomeCubeDto`

## Description

# 홈 화면에서 보여지는 배너 데이타 요청(큐브)

 - GET /home/banner/M00

 # 홈 화면에서 보여지는 배너 데이타 응답(큐브)

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|배너 고유 아이디|
 |title|string|배너 타이틀|
 |subtitle|string|배너 서브타이틀|
 |imageUrl|string|배너 이미지 URL|
 |contentType|string|배너 컨텐츠 타입|
 |contentId|string|배너 링크 아이디|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "배너(큐브) 타이틀1",
     "subTitle": "큐브 서브타이틀1",
     "imageUrl": "https://example.com/image.png",
     "contentType": "event",
     "contentId": "1",
   },
   {
     "id": "2",
     "title": "배너(큐브) 타이틀2",
     "subTitle": "큐브 서브타이틀2",
     "imageUrl": "https://example.com/image.png",
     "contentType": "event",
     "contentId": "2",
   }
 ]
 ```

## Dependencies

- _$HomeCubeDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

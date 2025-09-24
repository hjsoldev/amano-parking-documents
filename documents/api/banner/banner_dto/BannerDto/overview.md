# Overview for `BannerDto`

## Description

# 배너 목록 요청

 - GET /home/banner/M00 - 홈 화면에서 보여지는 큐브 배너
 - GET /home/banner/M01 - 홈 화면에서 보여지는 프로모션 배너
 - GET /home/banner/M02 - 홈 화면에서 보여지는 하단 가이드 배너
 - GET /home/banner/M03 - 이벤트 목록 상단에 보여지는 배너

 # 배너 목록 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|배너 고유 아이디|
 |title|string|배너 타이틀|
 |subtitle|string|배너 서브타이틀|
 |imageUrl|string|배너 이미지 URL|
 |linkType|string|이동 컨텐츠 링크|
 |linkId|string|이동 컨텐츠 아이디|

 - title, subtitle 값은 가이드 배너에 필요 - 이미지라면 해당 컬럼은 삭제
 - linkType 값(링크 타입)
   - event: 이벤트
   - notice: 공지
   - 배너를 클릭해서 이동할 컨텐츠가 어떤것이 있는지 확인 필요

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "배너(큐브) 타이틀1",
     "subTitle": "큐브 서브타이틀1",
     "imageUrl": "https://example.com/image.png",
     "linkType": "event",
     "linkId": "1",
   },
   {
     "id": "2",
     "title": "배너(큐브) 타이틀2",
     "subTitle": "큐브 서브타이틀2",
     "imageUrl": "https://example.com/image.png",
     "linkType": "event",
     "linkId": "2",
   }
 ]
 ```

## Dependencies

- _$BannerDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

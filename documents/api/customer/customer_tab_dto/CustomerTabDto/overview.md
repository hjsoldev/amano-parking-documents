# Overview for `CustomerTabDto`

## Description

# 고객센터 FAQ 탭 목록 요청
 ## 앱 실행시 최초 1회만 요청

 - GET /customers/tabs

 # 고객센터 FAQ 탭 목록 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|아이디(정렬 용도)|
 |type|string|탭 타입|
 |name|string|화면에 표시될 탭 이름|

 - type: name - 아마노에서 설정한 탭 타입, 탭 이름. customers/{type} 값으로 사용
   - app: 앱
   - product: 상품
   - refund: 환불
   - member: 회원
   - plots: 주차장

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "type": "app",
     "name": "앱",
   },
   {
     "id": "2",
     "type": "product",
     "name": "상품",
   }
 ]
 ```

## Dependencies

- _$CustomerTabDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

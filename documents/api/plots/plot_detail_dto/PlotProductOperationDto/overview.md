# Overview for `PlotProductOperationDto`

## Description

# 주차장 상품 운영 정보

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |name|string|상품 이름|
 |price|int|상품 가격|
 |discount|int|상품 할인 퍼센트|
 |status|string|상품 상태|
 |description|string|상품 설명|

 - 응답 파라미터 예시
 ```json

 {
   "name": "1시간권",
   "price": 2000,
   "discount": 50,
   "status": "sale",
   "description": "1시간권",
 }
 ```

 - status 값
   - sale: 판매중
   - closed: 판매종료

## Dependencies

- _$PlotProductOperationDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

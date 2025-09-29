# Overview for `ReceiptDto`

## Description

# 영수증 요청

 - GET /receipts/{id}

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|영수증 ID|

 - 요청 파라미터 예시

 ```json
 {
   "id": "1",
 }
 ```

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|영수증 ID|
  |productName|String|상품명|
  |paymentAmount|String|결제금액|
  |paymentMethod|String|결제방법|
  |paymentDate|String|결제일|
  |paymentNumber|String|승인번호|
  |businessName|String|사업자명|
  |businessNumber|String|사업자 등록번호|
  |representativeName|String|대표자명|
  |representativeAddress|String|대표자 주소|
  |createAt|String|날짜|

 - 응답 파라미터 예시

 ```json
 {
   "id": "1",
   "productName": "1시간권",
   "paymentAmount": "10000",
   "paymentMethod": "카드",
   "paymentDate": "2025-01-01",
   "paymentNumber": "1234567890",
   "businessName": "이마트",
   "businessNumber": "1234567890",
   "representativeName": "홍길동",
   "representativeAddress": "서울시 강남구 역삼동",
   "createAt": "2025-01-01"
 }
 ```

## Dependencies

- _$ReceiptDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`

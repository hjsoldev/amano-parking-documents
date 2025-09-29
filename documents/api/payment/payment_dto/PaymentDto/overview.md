# Overview for `PaymentDto`

## Description

# 결제 정보 요청

 - GET /payments/{id}

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|상품권 ID|

 - 요청 파라미터 예시

 ```json
 {
   "id": "1",
 }
 ```

 # 결제 정보 응답

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |ppOp|PlotProductOperationDto|상품 정보|
  |pleaseNotes|arr_String|안내 문구|
  |refundNotes|arr_String|환불 문구|

 - 응답 파라미터 예시

 ```json
 {
   "ppOp": {
     "id": "1",
     "name": "일일권",
     "price": 900000,
     "discount": 0,
     "status": "sale",
     "description": "일일권",
     "remainCnt": 10,
   },
   "pleaseNotes": ["본 상품의 유효기간은 구매 당일 00", "사전정산기 사용시 주차권 적용이 불가능 합니다.", "사용전 상품은 취소가 가능하나 입차시는 취소가 불가능한 상품 입니다.", "본 상품은 당일권 상품으로 00:00~23:59까지 사용이 가능한 상품 입니다.", "입출차 1회만 이용 가능하며, 출차 후 재입차시 현장 요금에 따라 추가 요금이 부과 됩니다.", "빠른 이용문의 : 아마노파킹 고객센터 0000-0000"],
   "refundNotes": ["본 상품의 유효기간은 구매 당일 00", "사전정산기 사용시 주차권 적용이 불가능 합니다.", "사용전 상품은 취소가 가능하나 입차시는 취소가 불가능한 상품 입니다.", "본 상품은 당일권 상품으로 00:00~23:59까지 사용이 가능한 상품 입니다.", "입출차 1회만 이용 가능하며, 출차 후 재입차시 현장 요금에 따라 추가 요금이 부과 됩니다.", "빠른 이용문의 : 아마노파킹 고객센터 0000-0000"],
 }
 ```

## Dependencies

- _$PaymentDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
### fromResponse


#### Parameters

- `response`: `dynamic`

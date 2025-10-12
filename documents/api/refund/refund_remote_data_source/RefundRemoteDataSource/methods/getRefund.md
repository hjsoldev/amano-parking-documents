# Method: `getRefund`

## Description

# 환불할 상품 정보 요청

 ## GET /refund/{id}

 ### 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|String|상품 상세정보 ID|

 # 환불할 상품 정보 응답

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|String|상품 상세정보 ID|
 |plotId|String|주차장 ID|
 |plotName|String|주차장 이름|
 |plotAddress|String|주차장 주소|
 |ticketId|String|주차권 ID|
 |ticketName|String|주차권 이름|
 |carNumber|String|차량번호|
 |paymentAmount|int|결제 금액|
 |validStartDate|String|유효 기간 시작일|
 |validEndDate|String|유효 기간 종료일|
 |availableTimeStart|String|이용 가능 시간 시작|
 |availableTimeEnd|String|이용 가능 시간 종료|
 |isSubscribed|bool|구독 상품 여부|
 |status|String|상태|

 ### status
 - complete: 완료
 - wait: 대기
 - cancel: 취소
 - expired: 만료
 - refund: 환불

 ### 응답 파라미터 예시

 ```json
 {
   "id": "1",
   "plotId": "1",
   "plotName": "주차장 이름",
   "plotAddress": "주차장 주소",
   "ticketId": "1",
   "ticketName": "주차권 이름",
   "carNumber": "1234",
   "paymentAmount": 10000,
   "validStartDate": "2025-01-01",
   "validEndDate": "2025-01-01",
   "availableTimeStart": "00:00",
   "availableTimeEnd": "24:00",
   "isSubscribed": false,
   "status": "complete"
 }
 ```

## Return Type
`Future<Either<AppException, WrapperDto<RefundDto>>>`

## Parameters

- `id`: `String`

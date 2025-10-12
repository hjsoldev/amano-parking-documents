# Method: `getRefundPolicy`

## Description

# 환불 정책 조회

 - GET /refund/policy

 - 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|String|상품 상세정보 ID|

 - 요청 파라미터 예시

 ```json
 {
   "id": "1",
 }
 ```
 # 환불 정책 응답

 - 응답 파라미터 예시

 ```json
 ['환불 정책 텍스트']
 ```

## Return Type
`Future<Either<AppException, WrapperDto<String>>>`


# Method: `getCustomer`

## Description

# FAQ 목록 요청

 ## GET /customer/{type}

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|아이디|
  |title|string|타이틀|
  |type|string|타입|
  |content|string|내용|
  |createAt|string|생성 날짜|

 ### type값은 /customer/tabs 요청 후 탭 타입 값으로 사용
 - app: 앱
 - product: 상품
 - refund: 환불
 - member: 회원
 - plots: 주차장

## Return Type
`Future<Either<AppException, WrapperDto<CustomerDto>>>`

## Parameters

- `tabType`: `String`

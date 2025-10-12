# Method: `getCustomerTabs`

## Description

# 고객센터 탭 목록 요청

 ## GET /customers/tabs

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|아이디(정렬 용도)|
 |type|string|탭 타입|
 |name|string|화면에 표시될 탭 이름|

 ### type: name - 아마노에서 설정한 탭 타입, 탭 이름. customers/{type} 값으로 사용
 - app: 앱
 - product: 상품
 - refund: 환불
 - member: 회원
 - plots: 주차장

## Return Type
`Future<Either<AppException, WrapperDto<CustomerTabDto>>>`


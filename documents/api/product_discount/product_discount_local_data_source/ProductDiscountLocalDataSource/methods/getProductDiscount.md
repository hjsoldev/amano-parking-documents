# Method: `getProductDiscount`

## Description

# 상품 할인 정보 데이타 예시

 ```json
 {
   "success": true,
   "message": "success",
   "meta": {
     "total": 4,
     "page": 1,
     "size": 10
   },
   "contents": [
     {
       "plotInfo": {
         "plotNm": "주차장 이름1",
         "addr": "주차장 주소1",
         "lngt": 127.111128,
         "ltd": 37.394981,
         "plotId": "1",
         "plotTicketType": "regular"
       },
       "plotOp": {
         "fstMin": 10,
         "fstAmt": 1000,
         "addChrgMin": 10,
         "addChrgAmt": 1000,
         "maxAmt": 10000
       },
       "pfOp": {
         "plotAliasNm": "주차장 별명1",
         "bildNm": "건물 이름1",
         "bildForms": ["public", "amano", "private", "mixed", "sub"],
         "plotForms": ["machine", "auto"],
         "totPakCnt": 100
       },
       "ppOp": {
         "id": "1",
         "name": "1시간권",
         "status": "sale",
         "description": "1시간권",
         "price": 1000,
         "discount": 50,
         "remainCnt": 10
       },
       "distance": 186
     },
     ...
   ]
 }
 ```

## Return Type
`Future<Either<AppException, WrapperDto<ProductDiscountDto>>>`

## Parameters

- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`

[![N|Solid](https://scontent.fcgk10-1.fna.fbcdn.net/v/t1.0-9/23561815_137329747033280_584519139072773078_n.jpg?oh=02aadb40d936a3d723ff2ae2ba8534ae&oe=5A61C728)](https://nodesource.com/products/nsolid)

# klikasuransiku_api

##### URLS
Development
```sh
http://www.simasjiwa.id/apiuat/
```

### Authentication
##### Endpoint
POST
```sh
/rest/v1/user/signin
```

#### URL Params Required:
| Params | Data Type |
|--|--|
|username| [text] |
|password|[text] |

#### Sample Call
```sh
$.ajax({
    url: "/rest/v1/user/signin",
    dataType: "json",
    type : "POST",
    data: {  
        "username": "your_username",
        "password":"your_password"
    },
    success : function(response) {
      console.log(response);
    }
  });
```

#### Sample Response
```sh
{
    "clienId": "5D89006A21776A45E050A8C04E0A33D8",
    "token": "56c217cd-0bea-4f64-8ae2-2db0a71fea35"
}
```

#### List of Products

##### Features
  - get all products

##### Endpoint
GET
```sh
/rest/v1/getlistproductpaspol
```
##### Sample Call:
QJuery Ajax Call 
```sh
$.ajax({
    url: "/rest/v1/getlistproductpaspol",
    headers: {
        "token": "5D89006A21776A45E050A8C04E0A33D8",
        "clienId":"56c217cd-0bea-4f64-8ae2-2db0a71fea35"
    }
    dataType: "json",
    type : "GET",
    success : function(response) {
      console.log(response);
    }
  });
```

##### Sample response:
success
```sh
{
    "listProduct": [
        {
            "productID": 1,
            "productPackageID": 1,
            "productType": "Personal Accident",
            "productName": "Simas Protection Complete Plan A",
            "productShortDescription": null,
            "productLongDescription": null,
            "benefit": null,
            "rop": null,
            "medicFee": null,
            "outpatient": null,
            "inpatient": null,
            "discount": null,
            "criticalilness": null,
            "guaranteeAcceptance": "yes",
            "compensationForDeath": "50000000",
            "listPremium": [
                {
                    "maxAge": 64,
                    "minAge": 1,
                    "premium": 456000
                }
            ],
            "additionalfee": null,
            "voucherCode": "ULTAH2ASJ",
            "discountType": null
        }
    ]
}
```

#### Product Inquiry

##### Features
  - Submit aplication and generate policy

##### Endpoint
POST
```sh
/rest/v1/productinquiry
```
##### Sample Call:
QJuery Ajax Call 
```sh
$.ajax({
    url: "/rest/v1/productinquiry",
    headers: {
        "token": "5D89006A21776A45E050A8C04E0A33D8",
        "clienId":"56c217cd-0bea-4f64-8ae2-2db0a71fea35"
    }
    dataType: "json",
    type : "POST",
    data: { 
          "productID": "1",
          "productPackageID": "1",
          "premium": "7500",
          "referenceCode": "PASPOLXX001",
          "transactionDate": "31/01/2017",
          "voucherCode": "ULTAH2ASJ",
          "policyHolder": {
            "firstName": "Jhon",
            "lastName": "Dhoe",
            "email": "jhon.doe@gmail.com",
            "phone": "085667788990",
            "NIK": "0923384958674349",
            "dob": "02/07/1990",
            "address": "Gedung Simas Jiwa Jl. Lombok No. 73 Jakarta Pusat 10350",
            "sex": "pria/wanita",
            "provinceID": "1",
            "cityID": "1"
          },
          "insured": {
            "firstName": "Jhon",
            "lastName": "Dhoe",
            "email": "jhon.doe@gmail.com",
            "phone": "085667788990",
            "NIK": "0923384958674349",
            "dob": "02/07/1990",
            "address": "Gedung Simas Jiwa Jl. Lombok No. 73 Jakarta Pusat 10350",
            "sex": "pria/wanita",
            "provinceID": "1",
            "cityID": "1"
          },
          "beneficiary": {
            "fullName": "Mika Dhoe",
            "relation": "adik",
            "dobBen": "02/07/1993"
          }
    },
    success : function(response) {
      console.log(response);
    }
  });
``

##### Sample response:
success
```sh
{
    "status": 200,
    "message": "Success",
    "data": {
        "referenceCode": "JAGAINXX001",
        "linkpolicy": "https://klikasuransiku.com/policydownload/?uid=5D89006A21776A45E050A8C04E0A33D8&pid=5D89006A21776A45E050A8C04E0A44D8"
    }
}
```

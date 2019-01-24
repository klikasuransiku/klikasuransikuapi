[![N|Solid](https://scontent.fcgk10-1.fna.fbcdn.net/v/t1.0-9/23561815_137329747033280_584519139072773078_n.jpg?oh=02aadb40d936a3d723ff2ae2ba8534ae&oe=5A61C728)](https://nodesource.com/products/nsolid)

# klikasuransiku_api

### Sign In
##### Endpoint
POST
```sh
/rest/v1/user/signin
```

#### URL Params Required:
##### -Body
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|username| [text] | Y | | |
|password|[text] | Y | | |

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
| Params | Data Type |
|--|--|
|clientId| [text] |
|token|[text] | 

```sh
{
    "clientId": "5D89996A21776A85E070U8C04E0A33D8",
    "token": "d64dcfe5-1cgg-4981-b7bc-7c8a1o589bda"
}
```

### List of Products
##### Features
  - get all products

##### Endpoint
GET
```sh
/rest/v1/getlistproductpaspol
```
#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | |

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

### List of Products PA
##### Features
  - get all products pa

##### Endpoint
GET
```sh
/rest/v1/getlistproductpa
```
#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | |

##### Sample Call:
QJuery Ajax Call 
```sh
$.ajax({
    url: "/rest/v1/getlistproductpa",
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
### List of Products Health
##### Features
  - get all products health

##### Endpoint
GET
```sh
/rest/v1/getlistproducthealth
```
#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | |

##### Sample Call:
QJuery Ajax Call 
```sh
$.ajax({
    url: "/rest/v1/getlistproducthealth",
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
### List of Products Life
##### Features
  - get all products Life

##### Endpoint
GET
```sh
/rest/v1/getlistproductlife
```
#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | |

##### Sample Call:
QJuery Ajax Call 
```sh
$.ajax({
    url: "/rest/v1/getlistproductlife",
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
#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | |

##### -Body
| Params | | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|--|
|productID| | [number] | Y | | |
|productPackageId| |[number] | Y | | |
|premium| |[number]| Y | | |
|referenceCode| |[text] | Y | 20 | |
|transactionDate| |[date] | Y | | format dd/MM/yyyy |
|voucherCode| |[text] | N | 20 | |
|policyHolder| |[jsonObject] | Y | | |
|| firstName |[text] | Y | 50 | |
|| lastName |[text] | N | 50 | |
|| email |[text] | Y | 50 | |
|| phone |[text] | Y | | |
|| NIK |[text] | Y | 16 | |
|| dob |[date] | Y | | format dd/MM/yyyy|
|| address |[text] | Y | 200 | |
|| sex |[text] | Y | | e.x pria, wanita |
|| provinceId |[text] | Y | |  |
|| cityId |[text] | Y | | |
|insured| |[jsonObject] | Y | | |
|| firstName |[text] | Y | 50 | |
|| lastName |[text] | N | 50 | |
|| email |[text] | Y | | 50 |
|| phone |[text] | Y | | |
|| NIK |[text] | Y | 16 | |
|| dob |[date] | Y | | format dd/MM/yyyy|
|| address |[text] | Y | 200 | |
|| sex |[text] | Y | | e.x pria, wanita |
|| provinceId |[text] | Y | |  |
|| cityId |[text] | Y | | |
|beneficiary| |[jsonObject] | Y | | |
|| fullName |[text] | Y | 50 | |
|| relation |[text] | Y | |e.x  istri, suami, anak, ayah, ibu, kakak, adik, orang tua|
|| dob |[date] | Y | | format dd/MM/yyyy|
|responsePertanyaan| |[jsonObject] | Y | | |
|| criticalIllness |[number] | Y | 50 | e.x 1 = yes; 0 = no|
|| activity |[number] | Y | | e.x 1 = yes; 0 = no|
|| extraPremi |[number] | Y | | e.x 1 = yes; 0 = no|
|| tinggi |[number] | Y | | in cm e.x 150 |
|| berat |[number] | Y | | in kg e.x  50|
|| inpatient |[number] | Y | | e.x 1 = yes; 0 = no|
|| healty |[number] | Y | | e.x 1 = yes; 0 = no|
|| pregnant |[number] | Y | | e.x 1 = yes; 0 = no|
|| prenatal |[number] | Y | | e.x 1 = yes; 0 = no|
|| insuredSex |[text] | Y | | e.x pria, wanita|

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
            "dob": "02/07/1993"
          },
          "responsePertanyaan":{
            "criticalIllness":0,
            "activity":0,
            "extraPremi":0,
            "tinggi":155,
            "berat":67,
            "inpatient":0,
            "healthy":1,
            "pregnant":1,
            "prenatal":1,
            "insuredSex":"female"
          }
    },
    success : function(response) {
      console.log(response);
    }
  });
```

##### Sample response:
success
```sh
{
    "status": 200,
    "message": "Success",
    "data": {
        "linkPolicy": "https://klikasuransiku.com/downloadDirectPolicy?transIdMerchant=2017122803041&uid=5D89006A21776A45E050A8C04E0A33D8&pid=e3d46ec4-277e-4eaf-addb-04d9c604ba3d",
        "referenceCode": "PASPOLXX001",
        "policyNo": "171950000017"
    }
}
```

failed
```sh
{
    "status": 400,
    "message": "Nomor Identitas Pemegang Polis tidak Valid",
    "data": null
}
```
```sh
{
    "status": 400,
    "message": "Nomor Identitas Tertanggung tidak Valid",
    "data": null
}
```
```sh
{
    "status": 400,
    "message": "Mohon maaf data tersebut masuk dalam daftar blacklist kami",
    "data": null
}
```
```sh
{
    "status": 400,
    "message": "Gagal Input Polis",
    "data": null
}
```
```sh
{
    "status": 400,
    "message": "Pertanyaan Kesehatan tidak Valid",
    "data": null
}
```
```sh
{
    "status": 400,
    "message": "Proses Simultan Gagal",
    "data": null
}
```

### Check Blacklist
##### Endpoint
POST
```sh
/rest/v1/cekblacklist
```

#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | 
##### -Body
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|name| [text] | Y | 50 | format dd/MM/yyyy |
|dob|[text] | Y | | format dd/MM/yyyy |

#### Sample Call
```sh
$.ajax({
    url: "/rest/v1/cekblacklist",
    dataType: "json",
    type : "POST",
    data: {  
        "name": "SUYATNO",
        "dob": "29/10/1964"
    },
    success : function(response) {
      console.log(response);
    }
  });
```

#### Sample Response
| Params | Data Type |
|--|--|
|name| [text] |
|dob|[text] | format dd/MM/yyyy
|hasil|[integer] 0 = untuk user tidak termasuk blacklist, 1 = jika user adalah user blacklist dan transaksi tidak boleh di lanjutkan

```sh
{
    "name": "SUYATNO",
    "dob": "29/10/1964",
    "hasil": 1
}
```

### Get List of Provinces

##### Features
  - get all Province

##### Endpoint
GET
```sh
/rest/v1/getProvince
```

#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | |

##### Sample Call:
QJuery Ajax Call 
```sh
$.ajax({
    url: "/rest/v1/getProvince",
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
    "provinceList": [
        {
            "provinceName": "-",
            "provinceId": "0"
        },
        {
            "provinceName": "BALI",
            "provinceId": "14"
        },
        {
            "provinceName": "BANGKA BELITUNG",
            "provinceId": "34"
        },
        {
            "provinceName": "BANTEN",
            "provinceId": "33"
        },
        {
            "provinceName": "BENGKULU",
            "provinceId": "8"
        },
        {
            "provinceName": "DAERAH ISTIMEWA YOGYAKARTA",
            "provinceId": "12"
        },
        {
            "provinceName": "DKI JAKARTA",
            "provinceId": "9"
        },
        {
            "provinceName": "TIMOR TIMUR",
            "provinceId": "27"
        }
    ]
}
```

### Get List City by Province

##### Features
  - get all City by Province

##### Endpoint
GET
```sh
/rest/v1/getCity/{province id}
```

#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | |

##### Sample Call:
QJuery Ajax Call 
```sh
$.ajax({
    url: "/rest/v1/getCity/10",
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
    "cityList": [
        {
            "provinceId": "10",
            "cityId": "299",
            "cityName": "BANDUNG"
        },
        {
            "provinceId": "10",
            "cityId": "692",
            "cityName": "BANDUNG BARAT"
        },
        {
            "provinceId": "10",
            "cityId": "6",
            "cityName": "BEKASI"
        },
        {
            "provinceId": "10",
            "cityId": "8",
            "cityName": "BOGOR"
        },
        {
            "provinceId": "10",
            "cityId": "303",
            "cityName": "CIAMIS"
        }
    ]
}
```
### Check Nik
##### Endpoint
POST
```sh
/rest/v1/cekNik
```

#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | 
##### -Body
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|noId| [text] | Y | 16 |  |
|dob|[text] | Y | | format dd/MM/yyyy |
|jenisKelamin|[text] | Y | | pria/male |

#### Sample Call
```sh
$.ajax({
    url: "/rest/v1/cekNik",
    dataType: "json",
    type : "POST",
    data: {
    "noId": "3173052910640005",
    "dob": "29\/10\/1964",
    "jenisKelamin": "pria"
},
    success : function(response) {
      console.log(response);
    }
  });
```

#### Sample Response
| Data Type | |
|--|--|
|[boolean] | true = valid, false = tidak valid|

```sh
true
```

### Check Response Pertanyaan
##### Endpoint
POST
```sh
/rest/v1/getValidatePertanyaan
```

#### URL Params Required:
##### -Header
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|token| [text] | Y | | |
|clienId|[text] | Y | | 
##### -Body
| Params | Data Type | Mandatory | Length | Description |
|--|--|--|--|--|
|criticalIllness| [number] | Y | | e.x 1 = yes; 0 = no |
|activity|[number] | Y | | e.x 1 = yes; 0 = no |
|extraPremi|[number] | Y | | e.x 1 = yes; 0 = no |
|tinggi| [number] | Y |  | e.x 1 = yes; 0 = no |
|berat|[number] | Y | | e.x 1 = yes; 0 = no |
|inpatient|[number] | Y | | e.x 1 = yes; 0 = no |
|healthy| [number] | Y |  | e.x 1 = yes; 0 = no |
|pregnant|[number] | Y | | e.x 1 = yes; 0 = no |
|insuredSex|[text] | Y | | e.x pria/male; wanita/female |

#### Sample Call
```sh
$.ajax({
    url: "/rest/v1/cekNik",
    dataType: "json",
    type : "POST",
    data: {
        "criticalIllness":0,
        "activity":0,
        "extraPremi":0,
        "tinggi":155,
        "berat":67,
        "inpatient":0,
        "healthy":1,
        "pregnant":1,
        "prenatal":1,
        "insuredSex":"female"
    },
    success : function(response) {
      console.log(response);
    }
  });
```

#### Sample Response
| Data Type | |
|--|--|
|[boolean] | true = valid, false = tidak valid|

```sh
true
```

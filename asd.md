### 1. GET /api/tribe/info/:tribeId

#### Description
Get tribe info by tribeId 

#### Resource
 > Please look forward to ☺

#### Authorization
none

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| tribeId |number| tribeId.| 

#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{
      tribeInfo:{
        id:'number',
        avatar:'string',
        description:'string',
        attention_sum:'number',
        member_sum:'number', 
      },
      hasAttention:'boolean',
      hasJoinTribe:'boolean'
    }
}
```

|Name|Type|Description| 
|----|----|--- | 
| tribeInfo |   JSON  | details of tribe | 
| tribeInfo -> id |   JSON  | id of tribe | 
| tribeInfo -> avatar |   String  | avatar of tribe | 
| tribeInfo -> description |   String  | description of tribe | 
| tribeInfo -> attention_sum |   Number  | how many of user attention the tribe| 
| tribeInfo -> member_sum |   Number  | how many of user in the tribe| 
|hasAttention  |  boolean|  express current user whether attention the tribe   |
|hasJoinTribe  |  boolean|  express current user whether join the tribe   |

### 2. POST /v1/user

#### Description
add a user.

#### Resource
 > POST [https://api.codemao.cn/v1/user](https://api.codemao.cn/v1/user)

#### Authorization
token

#### POST Parameters
|Name|Type|Description| 
|:—— |:——|—— | 
| userId |string| Unique identifier representing a specific product for a given latitude & longitude. For example, uberX in San Francisco will have a different product_id than uberX in Los Angeles. | 

#### Response
Status-code: 202 OK

```json

{   "request_id": "852b8fdd-4369-4659-9628-e122662ad257",   "product_id": "a1111c8c-c720-46c3-8534-2fcdd730040d",   "status": "processing",   "vehicle": null,   "driver": null,   "location": null,   "eta": 5,   "surge_multiplier": null }
```

|Name|Type|Description| 
|:—— |:——|—— | 
| product_id (optional) |   string  |  Unique identifier representing a specific product for a given latitude & longitude. For example, uberX in San Francisco will have a different product_id than uberX in Los Angeles.  | 
|short_description  |  string|    An abbreviated description of the product.    |

#### Error Responses
Status-code: 409 Conflict

```json
{
  "errors" : {
     "status": "409",
     "error": "conflict",
    "title": "…….."
  }
}
```

#### Possible Errors:
|Code|Error|Description| 
|:—— |:——|—— | 
|400 | bad request| Request param have some problem|
|401| unauthorized| User not login|
|403| forbidden| User is forbidden from making request at this time|
| 404 |   not_found  |  Unique identifier representing a specific product for a given latitude & longitude. For example, uberX in San Francisco will have a different product_id than uberX in Los Angeles.  |
|408| request timeout |Client |
|409|conflict||
|500 |internal_server_error|An unknown error has occurred. |

### 3. PUT /v1/user/{userId}

#### Description
edit the user info.

#### Resource
 > PUT [https://api.codemao.cn/v1/user/{userId}](https://api.codemao.cn/v1/user/{userId})

#### Authorization
can find user login token

#### Path Parameter
|Name|Type|Description| 
|:—— |:——|—— | 
| userId |string| Unique identifier representing a specific product for a given latitude & longitude. For example, uberX in San Francisco will have a different product_id than uberX in Los Angeles. | 

#### PUT Parameter
|Name|Type|Description| 
|:—— |:———|:——|—— | 
| age(optional) |number| Unique identifier representing a specific product for a given latitude & longitude. For example, uberX in San Francisco will have a different product_id than uberX in Los Angeles. | 

#### Response
Status-code: 200 OK

```json
{
  "age": "100"
}
```

|Name|Type|Description| 
|:—— |:——|—— | 
| age |   string  |  Unique identifier representing a specific product for a given latitude & longitude. For example, uberX in San Francisco will have a different product_id than uberX in Los Angeles.  | 
|short_description  |  string|    An abbreviated description of the product.    |

#### Error Responses
Status-code: 409 Conflict

```json
{
  "errors" : {
     "status": "409",
     "error": "conflict",
    "title": "…….."
  }
}
```

#### Possible Errors:
|Code|Error|Description| 
|:—— |:——|—— | 
|400 | bad request| Request param have some problem|
|401| unauthorized| User not login|
|403| forbidden| User is forbidden from making request at this time|
| 404 |   not_found  |  Unique identifier representing a specific product for a given latitude & longitude. For example, uberX in San Francisco will have a different product_id than uberX in Los Angeles.  |
|408| request timeout |Client |
|409|conflict||
|500 |internal_server_error|An unknown error has occurred. |

### 4. DELETE /v1/user/{userId}

#### Description
delete the user info.

#### Resource
 > DELETE [https://api.codemao.cn/v1/user/{userId}](https://api.codemao.cn/v1/user/{userId})

#### Authorization
only admin token

####Query Parameters


#### Response
Status-code: 204 OK


### 1. GET /api/work/tribe/info/:workId

#### Description
Get tribe info by workId 

#### Resource
 > Please look forward to ☺

#### Authorization
none

#### Path Parameters

#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{
      tribeList:[{
        id:'number',
        name:'string'
      }]
    }
}
```

|Name|Type|Description| 
|----|----|--- | 
| tribeList |   Array  | 作品所在的所有部落 | 
| tribeList -> id |   Number  | id of tribe | 
| tribeList -> name |   String  | name of tribe | 




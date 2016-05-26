### 1. GET /api/tribe/member/:tribeId

#### Description
Get all members in tribe by tribeId

#### Resource
 > Please look forward to ☺

#### Authorization
none

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| tribeId |number| tribeId| 
| amount |number| 一共要多少个成员 |
| offset |number| 跳过多少个成员 | 

#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{
      tribeMember:[{
        id:'number',
        avatar:'string',
        nickname:'string' 
      }]
    }
}
```

|Name|Type|Description| 
|----|----|--- | 
| tribeMember |   Array  | all members | 
| tribeMember -> id |   JSON  | id of tribe member | 
| tribeMember -> avatar |   String  | tribe member avatar | 
| tribeMember -> nickname |   String  | tribe member nickname | 

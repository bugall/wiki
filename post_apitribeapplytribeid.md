### 1. POST /api/tribe/apply/:tribeId

#### Description
Get all members in tribe by tribeId

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

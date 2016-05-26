### 1. GET /api/work/list

#### Description
Get tribe info by tribeId 

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
      workList:[{
        id:'number',
        thumbnail:'string',
        workName:'string',
        status:;'number',
        publish_time:'number'
      }]
    }
}
```

|Name|Type|Description| 
|----|----|--- | 
| workList |   Array  | all work of user | 
| workList -> id |   Number  | id of work | 
| workList -> thumbnail |   String  | preview of work | 
| workList -> workName |   String  | name of work | 
| workList -> status |   Number  | 1 为正常，-99 表示被删除| 
| tribeInfo -> member_sum |   Number  | how many of user in the tribe| 
|hasAttention  |  boolean|  express current user whether attention the tribe   |
|hasJoinTribe  |  boolean|  express current user whether join the tribe   |



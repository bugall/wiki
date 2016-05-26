### GET /api/tribe/work

#### Description
Get works in tribe
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
      workInfo:[{
        workId:'number',
        workName:'string',
        workPreview:'string',
        viewTimes:'number',
        attentionTimes:'number',
        praiseTimes:'number',
        userId:'number',
        userName:'string'
      }]
    }
}
```

|Name|Type|Description| 
|----|----|--- | 
| workInfo |   JSON  | details of work | 
| workInfo -> workId |   Number  | id of work | 
| workInfo -> workName |   String  | name of work | 
| workInfo -> workPreview |   String  | preview of work(is a cdn url) | 
| workInfo -> viewTimes |   Number  | how many of user has been see the work| 
| workInfo -> member_sum |   Number  | how many of user in the tribe| 
|hasAttention  |  boolean|  express current user whether attention the tribe   |
|hasJoinTribe  |  boolean|  express current user whether join the tribe   |
 
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
 
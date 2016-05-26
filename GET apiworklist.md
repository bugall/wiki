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
        publishTime:'number',
        updateTime:'number',
        collectionTime:'number',
        forkTimes:'number',
        viewTimes:'number',
        praiseTimes:'number',
        commentTimes:'number'
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
| workList -> publishTime |   Number  | 0表示未发布，非0表示已经发布，表示发布时间| 
| workList -> updateTime |   Number  | 最后一次修改的时间戳| 
| workList -> collectionTime |   Number  | 被收藏的次数 | 
| workList -> forkTimes |   Number  | 被再创作的次数 | 
| workList -> viewTimes |   Number  | 被浏览的次数 | 
| workList -> praiseTimes |   Number  | 被点赞的次数 | 
| workList -> commentTimes |   Number  | 评论的总数 | 




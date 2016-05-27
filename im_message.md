### 1.部落解散

```json
  {
    type:'tribe_has_been_disbanded',
    tribeId:'number',
    tribeName:'string'
  }
```
> 不生成动态,发送消息
 
### 2.申请加入部落
```json
  {
    type:'apply_join_tribe',
    senderId:'number',
    senderName:'string',
    tribeId:'number',
    tribeName:'string',
    logicYes:'Url',
    logicNo:'Url'
  }
```
> 不生成动态,发送消息

### 3.邀请加入部落
```json
  {
    type:'invita_join_tribe',
    senderId:'number',
    senderName:'string',
    tribeId:'number',
    tribeName:'string',
    logicYes:'Url',
    logicNo:'Url'
  }
```
> 不生成动态,发送消息

### 4.部落成员提升为管理员
```json
  {
    type:'upgrade_to_manager',
    tribeId:'number',
    tribeName:'string'
  }
```
> 生成动态,发送消息

### 5.部落成员将为普通成员
```json
  {
    type:'downgrade_to_manager',
    tribeId:'number',
    tribeName:'string'
  }
```
> 生成动态,发送消息

### 6.删除部落成员
```json
  {
    type:'delete_user_from_tribe',
    userId:'number',
    userName:'string',
    tribeId:'number',
    tribeName:'string'
  }
```
> 生成动态,发送消息

### 7.用户退出部落
```json
  {
    type:'member_quit_from_tribe',
    userId:'number',
    userName:'string',
  }
```
> 生成动态,不发送消息

### 8.有新用户加入部落
```json
  {
    type:'join_tribe',
    userId:'number',
    userName:'string',
    tribeId:'number',
    tribeName:'string'
  }
```
> 生成动态,发送消息

### 9.拒绝用户加入部落
```json
  {
    type:'refuse_apply_join_tribe',
    tribeId:'number',
    tribeName:'string'
  }
```
> 不生成动态,发送消息

### 10.新作品加入部落
```json
  {
    type:'add_work_to_tribe',
    userId:'number',
    userName:'string',
    tribeId:'number',
    tribeName:'string',
    workId:'number',
    workName:'string',
  }
```
> 生成动态,发送消息
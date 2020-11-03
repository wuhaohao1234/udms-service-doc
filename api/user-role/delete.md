# 移除用户的某个角色

#### ```post /api/user-role/delete```
##### ```v1.0.0```

移除用户的某个角色，删除其对应的关联关系

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} user_id``` 用户id
  * ```{integer} role_id``` 角色id

<br />

## 成功响应
无

<br />

## 错误代码
全局错误代码参考```global.md```。

#### ```ERR_NOT_FOUND```
移除用户的某个角色失败，未找到这个关联关系
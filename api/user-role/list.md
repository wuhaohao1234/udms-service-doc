# 查询用户的所有角色

#### ```GET /api/user-role/list```
##### ```v1.0.0```
返回某个用户的所具有的所有角色

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} user_id``` 用户id

<br />

## 成功响应
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object[]}``` 没查到数据应返回空数组
  * ```{integer} role_id``` 角色id
  * ```{integer} name``` 角色名称

<br />

## 错误代码
全局错误代码参考```global.md```。
# 给某个用户添加角色

#### ```POST /api/user-role/add```
##### ```v1.0.0```

给某个用户添加一个特定的角色，建立关联关系

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
# 给角色添加权限

#### ```POST /api/role-authority/add```
##### ```v1.0.0```

给某个角色添加一项权限

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} role_id``` 角色id
  * ```{integer} auth``` 这个角色对应的某个权限，参考权限标准文件

<br />

## 成功响应
无

<br />

## 错误代码
全局错误代码参考```global.md```。
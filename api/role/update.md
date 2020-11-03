# 更新角色

#### ```POST /api/role/update```
##### ```v1.0.0```
更新某个角色的数据

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} id``` 角色ID
  * ```{string|undefined} name``` 角色名称

#### 验证规则
1. 除```id```外至少要设置一个值才能使更新有意义

<br />

## 错误代码
全局错误代码参考```global.md```。

#### ```ERR_NOT_FOUND```
角色没有找到时设置这个错误。
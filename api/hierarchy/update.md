# 更新某个组织层级

#### ```POST /api/hierarchy/update```
##### ```v1.0.0```
更新某个组织层级的数据

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} id``` 查找到要更新的组织层级ID
  * ```{string|undefined} name``` 组织层级名称

#### 验证规则
1. ```id```之外的字段至少要设置一个才能使本次更新有意义

<br />

## 错误代码
全局错误代码参考```global.md```。

#### ```ERR_NOT_FOUND```
组织层级没有找到时设置这个错误。
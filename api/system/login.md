# 用户登陆

#### ```POST /api/system/login```
##### ```v1.0.0```
在使用用户相关的功能之前需要先使用登陆API完成token的签发，登陆以后需要将信息按需缓存在客户端，以维持用户的登陆状态。

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{string} mode``` 登陆模式，以下列举取值范围
    * ```un```: 员工用户名登陆
  * ```{string} auth``` 用于登陆的标识信息，```mode```为```un```时代表用户名
  * ```{string} password``` 用于登陆的密码信息，```mode```为```un```时代表密码

<br />

## 成功响应
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} id``` 当前登陆的用户ID
  * ```{string} token``` 给当前登陆的用户签发的一个令牌，后续交互需要携带
  * ```{string} register_name``` 用户名

<br />

## 错误代码
全局错误代码参考```global.md```。

#### ```ERR_LOGIN_FAILED```
登陆失败，一定是由于用户名或密码无相应匹配的用户才会发送，否则不应发送此代码。
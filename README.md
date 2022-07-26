## 短链接服务

## https://tourl.cc/

> 注意：默认有效期为30天。 无需注册即可使用 



### 跳转URL
__GET__ __/{shortId}__

参数说明

|参数|类型|说明|
|---|---|---|
|shortId|string|短链接id|

> 会判断 {shortId} 是否存在如果存在并且不过期直接 通过 head 302 found 跳转到指定地址

### 创建短链接
__POST__ __/api/v1/url__

参数说明
```json
{
  "url": "https://xcv.cdf.com/asfdi8j2f/2f23f32f?asdf8=23ferwq"
}
```
|参数|类型|说明|
|---|----|---|
|url|string|生成短链接url|

返回说明
```json
{
    "short_url": "https://tourl.cc/asjdfi32",
    "expire_time": "2022-05-02 00:00:00"
}
```
| 字段 | 类型 | 说明 |
|-----|------|-----|
|short_url|string|生成的短链接地址|
|expire_time|string|过期时间|


> 如需其他功能可以给我留言



    
##### 简要描述

- 全局相关参数和配置

##### 请求基础URL(BASE_URL)
- ` https://gamecenter-api.xx.com `
  
##### 请求方式
- POST 

##### 请求加密方式
- RSA 

##### 返回加密方式
- RSA 

##### 全局参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|time |是  |int |本地时间戳，单位:秒   |
|nonce |是  |string | 随机字符串   |
|encrypt_data |是  |string | RSA加密后数据   |
|sign |是  |string | MD5加密后数据   |

##### 登录后请求头

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|token |是  |string |登录后TOKEN   |

##### RSA加密全局参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|game_id |是  |int |游戏ID   |
|agent_id |是  |int | 渠道ID    |
|site_id     |是  |int | 广告位ID    |
|device_id     |是  |string | 设备码，安卓为IMEI，iOS为idfa    |
|android_id     |是  |string | 安卓ID    |
|system_version     |是  |string | 系统版本号    |
|model     |是  |string | 机型    |
|mnos     |是  |int | 网络类型    |
|app_version_code     |是  |int | APP整形版本号    |
|sdk_version_code     |是  |int | SDK整形版本号    |
|user_id     |否  |int | 登陆后必填    |

##### 返回示例 

``` 
  {
    "code": 1,
	"msg":"success",
    "info": {
    },
	"lists":[
	
	],
	"request_id":"sfdsfdsfdfdsf"
  }
```

##### 返回参数说明 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|code |int   |状态码。1：成功，非1，失败  |
|msg |string   |消息提示  |
|info |json   |json格式，业务不同返回不同  |
|lists |[json]   |json数组，业务不同返回不同  |

##### 备注 





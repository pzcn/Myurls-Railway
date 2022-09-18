# Myurls-Railway

在 [Railway](https://railway.app/) 上运行 [Myurls](https://github.com/CareyWang/MyUrls) 短网址程序

## Installation

### 部署

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/rNhsEU?referralCode=MikuFun)

- 点击上方图片跳转 Railway
- 登陆你的 Github 账号
- 填写你要创建的库名  
- 添加自定义域名至 `DOMAIN` 
- 点击部署
- 配置自定义域名以通过此域名访问

🎉🎉🎉 完成！🎉🎉🎉

### 绑定域名
> 简述，具体配置请参考[官方文档](https://docs.railway.app/deploy/exposing-your-app#lets-encrypt-ssl-certificates)。

- 在 Cloudflare 中添加 `Cname` 解析指向 `yourapp.yourrailwayproject.com` 
    - 可能长这样 `https://xxxx-xxxxx.xx.railway.app/`
- 并配置 `SSL/TLS` 的 **加密模式** 为 **完全** 或 **完全（严格）**
- 在 `Railway` 的 `Settings - Domains` 中接入该域名


---

#### 参数说明：

- `DOMAIN` 
    - 短链接域名，必填，不需要添加https:// (如 abc.com)
- `TTL` 
    - 短链接有效期（默认 180，单位：天，不用修改）
- `PORT` 
    - 端口（默认 80，不用修改）
- `RDSHOST`
    - Redis 的域名
- `RDSPORT`
    - Redis 的端口
- `RDSPASSWORD`
    - Redis 的密码


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Log
- 2022-09-18
    - `[^]`：原本的模板报错 “template is not an available Railway plugin”，故重新配置了一个模板。还测试了挺多次的，还好能看懂点 sh 脚本。sh脚本改了几个变量名以搭配模板使用，请自行查看。
    另外模板加入了我的推广码，觉得膈应请[点我部署](https://railway.app/new/template/rNhsEU)。

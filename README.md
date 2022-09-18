# Myurls-Railway

在 [Railway](https://railway.app/) 上运行 [Myurls](https://github.com/CareyWang/MyUrls) 短网址程序

## Installation

### 部署

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/rNhsEU?referralCode=MikuFun)

- 点击上方图片跳转 Railway
- 登陆你的 Github 账号
- 填写你要创建的库名  
- 添加自定义域名至 `DOMAIN` 

参数说明：

- `DOMAIN` - 短链接域名，必填项，不需要添加https:// (如 abc.com)
- `TTL` - 短链接有效期，单位(天)，默认180天 (default 180)
- `PORT` - 端口，保持80，请勿修改

### 添加域名

- 在 Cloudflare 中添加 `Cname` 解析指向 `myurls-production.up.railway.app`
- 并配置 `SSL/TLS` 的 **加密模式** 为 **完全** 或 **完全（严格）**
- 在 `Railway` 的 `Settings - Domains` 中接入该域名
> 具体配置请参考[官方文档](https://docs.railway.app/deploy/exposing-your-app#lets-encrypt-ssl-certificates)。

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Log
- 2022-09-10
    - `[^]`：原本一键部署报错 “template is not an available Railway plugin”，故重新构建了一个脚本。原本失效愿意应该和 Railway 有关。
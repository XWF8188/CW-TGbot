# CF-Workers-TGbot

## 🛠️ 部署到 Cloudflare Workers
1. 在 Cloudflare Worker 控制台中创建一个新的 Worker。
2. 将 [_worker.js](https://github.com/cmliu/CF-Workers-TGbot/blob/main/_worker.js)  的内容粘贴到 Worker 编辑器中。

## 📦 部署到 Cloudflare Pages
1. 在 Cloudflare Pages 上创建新项目，指定此仓库地址。
2. 部署后，通过 Pages 提供的域名访问即可（如设置域名 CNAME 到 Pages）。

## ⚠️ 使用说明
- 本示例假设域名为：`api.tg.090227.xyz`
- 使用反代 TG API 示例：  
  `https://api.tg.090227.xyz/bot${BotToken}/sendMessage?chat_id=${ChatID}&parse_mode=HTML&text=test`
- 如已在环境变量中设置 **TGTOKEN**，可直接调用内置通知机器人：  
  `https://api.tg.090227.xyz/sendMessage?chat_id=${ChatID}&parse_mode=HTML&text=test`
- 首次部署后，需访问以下链接对进行通知机器人初始化：  
  `https://api.tg.090227.xyz/${TGTOKEN}`

## 📋 变量说明
| 变量名 | 示例 | 备注 | 
|-|-|-|
| TGTOKEN | `6894123456:XXXXXXXXXX0qExVsBPUhHDAbXXXXXqWXgBA` | TG机器人token | 

# 🙏 致谢
GPT
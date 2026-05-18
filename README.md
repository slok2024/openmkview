OpenMKView-Cloudflare
这是一个基于 Next.js 15 构建的高效 Markdown 全栈轻量视窗与管理系统。项目经过 OpenNext (Cloudflare Adapter) 的深度优化与重构，已完全适配 Cloudflare 生态。

项目移除了本地笨重的开发环境依赖，通过编译成果提炼，支持在 Cloudflare Workers / Pages 上进行纯零成本、无服务器（Serverless）边缘全栈部署。

✨ 项目特性
全栈架构：基于 Next.js 15 开发，完美融合前端视窗与后端 API 路由。

边缘原生：完美适配 Cloudflare Workers 运行环境，享受极致的全球分布式加载速度。

极简交接：无需复杂的 npm install、Next build 以及多版本依赖冲突调整，开箱即用。

🚀 30秒一键傻瓜部署指南 (发布版)
如果你下载的是我们已经打包编译好的 Release 成果包，你完全不需要配置任何前端开发环境，只需两步即可将其推送到你自己的 Cloudflare 账号中：

前提条件
部署机需要安装 Node.js 环境（用于调用官方部署工具）。如未安装，请前往 nodejs.org 下载最新的 LTS 稳定版。

部署步骤
下载并解压 编译成果压缩包（内含 .open-next 文件夹、wrangler.toml 与 一键部署.bat）。

双击运行 目录下的 一键部署.bat。

此时会弹出浏览器登录网页，允许授权登录您的 Cloudflare 账号。

脚本会自动将全栈成果上传至您的账户，并在命令行最后打印出分配给您的免费专属域名（例如 openmkview.xxxx.workers.dev），点击即可直接访问！

🛠️ 后端自定义修改 (Wrangler.toml)
如果你需要修改发布在云端的项目名称，可以直接用记事本打开 wrangler.toml，修改第一行的 name 字段：

Ini, TOML
name = "你的自定义项目名称"

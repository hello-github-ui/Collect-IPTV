## 📡Collect-IPTV
初始版本基于 DeepSeek 与 ChatGPT 生成，最新版本使用 Gemini 与 GPT-5.3-Codex 持续优化；依托 GitHub 服务器进行源地址可用性与延迟测试，网页已更新台标展示，并支持去重与优选低延迟最佳 URL，M3U 播放列表每 4 小时自动更新。
&gt; ⚠️ 特别说明：因使用 GitHub 服务器，**不保证国内网络环境下的链接速度与可用性**。  
&gt; ⚠️ 所有频道的完整性与有效性高度依赖上游网络资源；若上游频道源大面积失效，自动更新时可能会被可用性检测过滤。

---
## 👤作者信息
- 作者：hello-github-ui
- 项目地址：https://github.com/hello-github-ui/Collect-IPTV
- 默认分支：master

---
## 📢 免责声明（个人学习测试专用）
本项目仅用于**网络协议、爬虫技术、自动化脚本开发等个人学习与测试用途**，不用于任何商业、盈利及违规用途。
- 所有节目源均来自互联网公开可访问链接，项目本身不生产、不存储、不篡改任何媒体内容。  
- 严禁将本项目及生成的播放列表用于商业传播、二次分发、公开分享等行为。  
- 所有频道版权均归原版权方所有，使用前请确保符合当地法律法规。  
- 因违规使用本项目产生的任何法律责任、版权纠纷，均由使用者自行承担。
详细免责声明请参阅 [`DISCLAIMER.md`](./DISCLAIMER.md)。

---
## 📺️TV station list
https://hello-github-ui.github.io/Collect-IPTV/

---
## 🚀部署指南

### GitHub Pages 部署

1. **Fork 项目**
   - 访问 https://github.com/hello-github-ui/Collect-IPTV
   - 点击右上角的 "Fork" 按钮将项目复制到自己的账号

2. **设置默认分支为 master**
   - 进入你 Fork 后的仓库设置
   - 找到 "Branches" 选项
   - 将默认分支设置为 master

3. **启用 GitHub Actions**
   - 进入仓库的 "Actions" 标签页
   - 点击 "I understand my workflows, go ahead and enable them" 启用工作流
   - 仓库会自动配置两个工作流：
     - `IPTV Daily Update`：每4小时自动更新播放列表
     - `Deploy static content to Pages`：部署静态页面到 GitHub Pages

4. **配置 GitHub Pages**
   - 进入仓库设置 (Settings)
   - 找到 "Pages" 选项
   - 在 "Build and deployment" 部分：
     - Source: 选择 "Deploy from a branch"
     - Branch: 选择 `gh-pages` 分支，文件夹选择 `/ (root)`
     - 点击 "Save"
   
5. **触发首次部署**
   - 进入 Actions 标签页
   - 选择 "IPTV Daily Update" 工作流
   - 点击 "Run workflow" 手动触发一次运行

### Vercel 部署

1. **连接 GitHub 仓库**
   - 访问 https://vercel.com 并登录
   - 点击 "Add New" → "Project"
   - 导入你的 Collect-IPTV 仓库

2. **配置项目设置**
   - 在 "Configure Project" 页面：
     - Framework Preset: 选择 "Other"
     - Root Directory: 保持为 `.`
     - Output Directory: 设置为 `.github/workflows`
     - Install Command: 留空
     - Build Command: 设置为 `cp best_sorted.m3u best_sorted.m3u8 .github/workflows/`
   
3. **部署**
   - 点击 "Deploy" 开始部署
   - 部署完成后，Vercel 会提供一个访问链接

4. **自动部署**
   - Vercel 会自动监听你的 master 分支
   - 每次推送到 master 都会自动触发重新部署

---
## ⏱️Last Run Time
&lt;!-- Last Run Time --&gt; 2026-05-18 04:42:46 CST

---
## 🔗Generated File Link
&lt;!-- Generated File Link M3U --&gt; [View M3U File](https://hello-github-ui.github.io/Collect-IPTV/best_sorted.m3u)

&lt;!-- Generated File Link M3U8 --&gt; [View M3U8 File](https://hello-github-ui.github.io/Collect-IPTV/best_sorted.m3u8)

---
## 💡 使用说明
1. 直接在播放器中订阅上方 `best_sorted.m3u` 或 `best_sorted.m3u8` 链接，即可获取最新节目源内容
2. 也可以打开链接后保存文件，再导入支持 IPTV 的播放器（如 Kodi、PotPlayer、Perfect Player 等）
3. 节目源每 4 小时自动更新，建议定期刷新订阅

---
## ⭐️Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hello-github-ui/Collect-IPTV&amp;type=Date)](https://star-history.com/#hello-github-ui/Collect-IPTV)

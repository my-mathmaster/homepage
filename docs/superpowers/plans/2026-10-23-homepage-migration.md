# 个人主页迁移计划

**目标：** 将 `afy03/afy03.github.io` 的主页代码和完整 Git 历史复制至主账户的独立公开仓库 `my-mathmaster/homepage`，使用 `afywty.top` 对外访问。

**架构：** 主页沿用现有 Jekyll 和 GitHub Pages 分支构建。博客也迁移至 GitHub Pages：源码保留在私有仓库 `my-mathmaster/my-mathmaster.github.io`，生成的静态文件发布至新的公开仓库 `my-mathmaster/blog`，目标域名为 `blog.afywty.top`。本阶段先迁移主页；不删除旧站，不覆盖主账户已有仓库。

**技术：** Git、GitHub CLI、Jekyll、GitHub Pages、阿里云 DNS。

## 执行步骤

- [x] 克隆主页、确认源码版本与完整历史，并生成独立 Git bundle 备份。
- [x] 确认原仓库属于 fork 网络，主账户已有同源 fork；选择创建独立仓库以避免转移限制。
- [x] 完成主账户 GitHub CLI 网页授权，读取登录身份确认是 `my-mathmaster`。
- [x] 检查目标仓库是否已存在；只有不存在时创建公开仓库，若存在则先检查内容，禁止覆盖。
- [x] 修改 `_config.yml`：repository 指向 `my-mathmaster/homepage`，url 为 `https://afywty.top`，baseurl 为空。
- [x] 新建根目录 `CNAME`，内容为 `afywty.top`。
- [x] 检查 YAML、域名和 diff；GitHub Pages 的完整 Jekyll 构建及部署成功。
- [x] 保留旧站远程地址，增加新仓库 remote；以普通非强制 push 将 `migrate/main-account:main` 推送至目标，验证旧提交仍为目标 main 的祖先。
- [x] 配置新仓库 Pages 来源为 main 分支根目录，检查构建及部署结果。
- [x] 在主页导航中添加指向 `https://blog.afywty.top/` 的 Blog 链接。
- [ ] 查询 DNS 当前状态及现有网站用途，若根域名当前提供博客，先让博客子域名正常访问再切换根域名；修改网站对应的 A/CNAME 记录需要域名控制台授权或用户操作，无需索取明文密钥。
- [ ] DNS 就绪后检查主页、CSS、图片和 HTTPS；记录未完成的权限或配置环节。

## 配置范围与验收

- `_config.yml`：仅变更站点仓库和 URL 配置。
- `CNAME`：声明主页自定义域名。
- `_data/navigation.yml`：添加博客导航链接。
- `docs/superpowers/plans/2026-10-23-homepage-migration.md`：记录执行状态；docs 已被站点构建排除。
- 原始提交 `8cfdfbfb6bb6257558d2b1c2995a69c8117059b7` 必须是新仓库 main 的祖先；保留原作者、许可证及历史。
- 新仓库应为独立公开仓库，保留源仓库现有内容；GitHub stars、secrets 等仓库元数据不随代码复制。
- 旧站继续保留，待新站正常后再决定跳转。阿里云 DNS 权限独立于 GitHub 登录；旧 Vercel 博客在域名切换前继续提供服务。
- 原有 Scholar 采集工作流需要 GOOGLE_SCHOLAR_ID；未配置时如失败应与 Pages 构建结果分开报告，不虚报全部工作流通过。
- 本地没有 Ruby/Bundler，不将静态配置检查误报为 Jekyll 构建通过。

## 当前状态

- 2026-10-23：迁移配置提交为 `b7c595e`；配置和 Git 历史验证通过，已推送至新的独立公开仓库 `my-mathmaster/homepage`，当前远端 main 为 `39590b1`。
- GitHub CLI 已以 `my-mathmaster` 完成授权，仓库 Pages 已设置为 main 分支根目录构建，自定义域名为 `afywty.top`。
- GitHub Pages 运行 `39824301643` 的构建和部署均成功；构建产物的标题、canonical URL、CSS、头像和 CNAME 已验证。
- 用户已选择主页和博客均使用 GitHub Pages；博客源码保持私有，仅将生成产物发布至新的公开仓库 `my-mathmaster/blog`。
- `afywty.top` 目前重定向到 `www.afywty.top`，其 Vercel 页面标题为「爱飞鱼的blog - 分享知识，探索世界」。切换根域名前需先处理博客子域名。
- DNS 切换和自定义域名 HTTPS 验证尚未完成；当前根域名和 www 仍提供旧 Vercel 博客。
- 现有源仓库及线上站点均未修改。

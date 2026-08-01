# We-MP-RSS 项目变更总结

> 从 1.4.6 到 1.4.8 的完整变更记录
> 
> 本文档基于 Git 历史自动生成，详细记录了从 e8255ab9 (2025-08-23) 到 27b672d1 (2026-01-19) 之间的所有代码变更

## 📌 概览

本次版本迭代跨越约5个月时间，包含 **167 个提交**，涉及 **+5961/-2170** 行代码变更。主要完成了以下重大功能升级：

- 🗄️ **数据库扩展**：新增 PostgreSQL 支持
- 🌐 **浏览器升级**：从 Firefox WebDriver 迁移到 Playwright
- 📤 **导出增强**：支持 PDF、Word、Markdown、HTML、JSON 五种格式
- 💻 **跨平台支持**：增加 ARM64 架构兼容性
- 🏷️ **标签功能**：导入导出、自定义 LOGO、预览等多项改进
- ✅ **阅读管理**：新增文章已读状态跟踪
- 🔔 **消息通知**：浏览器桌面通知功能
- 🔐 **安全加固**：CSRF 防护及多项安全漏洞修复
- ⚡ **性能优化**：任务调度、资源管理等多方面优化

## 📋 版本信息

| 项目 | 内容 |
| --- | --- |
| **起始版本** | 1.4.6 - 增加标签订阅功能 (e8255ab9) |
| **结束版本** | 1.4.8-Fix (27b672d1) |
| **开发时间** | 2025年8月23日 - 2026年1月19日 (约5个月) |
| **提交数量** | 167 个提交 |
| **代码变更** | +5961 / -2170 |

## 🚀 主要功能亮点

✅ **PostgreSQL 数据库支持** - 新增 PostgreSQL 作为数据库选项
✅ **Playwright 浏览器引擎** - 从 Firefox WebDriver 升级到 Playwright
✅ **多格式导出** - 支持 PDF、Word、Markdown、HTML、JSON 格式导出
✅ **ARM64 架构支持** - 支持 ARM64 处理器，适配更多设备
✅ **标签系统增强** - 标签导入导出、自定义 LOGO、预览功能
✅ **已读状态管理** - 新增文章已读功能
✅ **浏览器通知** - 新文章浏览器提醒
✅ **API 扫码登录** - 优化登录体验
✅ **安全性增强** - CSRF 防护等安全改进

## 📑 详细目录

1. [PostgreSQL支持](#-postgresql支持) (4 个提交)
2. [浏览器引擎升级](#-浏览器引擎升级) (7 个提交)
3. [导出功能](#-导出功能) (8 个提交)
4. [标签管理](#-标签管理) (17 个提交)
5. [ARM64支持](#-arm64支持) (9 个提交)
6. [通知系统](#-通知系统) (2 个提交)
7. [已读功能](#-已读功能) (3 个提交)
8. [API扫码登录](#-api扫码登录) (2 个提交)
9. [任务调度](#-任务调度) (5 个提交)
10. [安全性](#-安全性) (4 个提交)
11. [UI优化](#-ui优化) (2 个提交)
12. [文档](#-文档) (6 个提交)
13. [性能优化](#-性能优化) (4 个提交)
14. [Bug修复](#-bug修复) (55 个提交)
15. [其他](#-其他) (20 个提交)

---

## 🔧 PostgreSQL支持

**功能描述**: 为系统添加 PostgreSQL 数据库支持，扩展数据库选项

**提交数量**: 4 个

**代码变更**: +71 / -78

### 关键提交详情

#### 1. 1.4.6 增加postgres支持

- 📅 **日期**: 2025-10-10
- 👤 **作者**: t@123654
- 🔗 **提交**: `c8ccc5cc`
- 📊 **变更**: +47 / -14

**修改的文件**:

- `1.txt` (+11/-0)
- `Dockerfiles/py3.13.1/requirements.txt` (+3/-2)
- `core/models/base.py` (+1/-1)
- `data_sync.py` (+26/-8)
- `driver/wx.py` (+3/-1)
- `requirements.txt` (+3/-2)

#### 2. 1.4.6 增加postgres支持

- 📅 **日期**: 2025-10-10
- 👤 **作者**: t@123654
- 🔗 **提交**: `4d0ac560`
- 📊 **变更**: +0 / -57

**修改的文件**:

- `1.txt` (+0/-57)

#### 3. 1.4.6 增加postgres支持

- 📅 **日期**: 2025-10-10
- 👤 **作者**: t@123654
- 🔗 **提交**: `f08b01ef`
- 📊 **变更**: +10 / -1

**修改的文件**:

- `ReadMe.md` (+8/-0)
- `config.example.yaml` (+2/-1)

#### 4. 1.4.6 增加postgres支持

- 📅 **日期**: 2025-10-10
- 👤 **作者**: t@123654
- 🔗 **提交**: `cc85112b`
- 📊 **变更**: +14 / -6

**修改的文件**:

- `ReadMe.md` (+14/-6)

---

## 🔧 浏览器引擎升级

**功能描述**: 从 Firefox WebDriver 迁移到 Playwright，提升浏览器自动化能力

**提交数量**: 7 个

**代码变更**: +141 / -97

### 关键提交详情

#### 1. "1.4.7 "调整为playwright驱动""

- 📅 **日期**: 2025-11-05
- 👤 **作者**: RACH
- 🔗 **提交**: `d97f4329`
- 📊 **变更**: +63 / -21

**修改的文件**:

- `apis/auth.py` (+1/-1)
- `core/wx/__init__.py` (+1/-1)
- `core/wx/base.py` (+4/-1)
- `core/wx/{wx1.py => model/api.py}` (+1/-1)
- `core/wx/{wx3.py => model/app.py}` (+1/-1)
- `core/wx/{wx2.py => model/web.py}` (+1/-1)
- `driver/base.py` (+1/-0)
- `.../{firefox_driver.py => firefox_driver.py.del}` (+4/-2)
- _(还有 7 个文件)_

#### 2. "1.4.7 调整为playwright驱动"

- 📅 **日期**: 2025-11-05
- 👤 **作者**: RACH
- 🔗 **提交**: `bc2c38b0`
- 📊 **变更**: +1 / -1

**修改的文件**:

- `publish.bat` (+1/-1)

#### 3. "1.4.8 浏览器内核更换为playwright"

- 📅 **日期**: 2025-11-07
- 👤 **作者**: RACH
- 🔗 **提交**: `1e7272e1`
- 📊 **变更**: +1 / -1

**修改的文件**:

- `.github/workflows/release.yaml` (+1/-1)

#### 4. "1.4.8 当不使用web浏览器方式时不安装playwright"

- 📅 **日期**: 2025-11-07
- 👤 **作者**: RACH
- 🔗 **提交**: `fa4a7c63`
- 📊 **变更**: +24 / -25

**修改的文件**:

- `dock_build.bat` (+1/-1)
- `driver/playwright_driver.py` (+22/-22)
- `start.sh` (+0/-1)
- `test_article.py` (+1/-1)

#### 5. "1.4.8 当不使用web浏览器方式时不安装playwright"

- 📅 **日期**: 2025-11-07
- 👤 **作者**: RACH
- 🔗 **提交**: `9c143bf4`
- 📊 **变更**: +2 / -1

**修改的文件**:

- `README.zh-CN.md` (+1/-0)
- `driver/playwright_driver.py` (+1/-1)

#### 6. "1.4.8 当不使用web浏览器方式时不安装playwright"

- 📅 **日期**: 2025-11-07
- 👤 **作者**: RACH
- 🔗 **提交**: `7fe30551`
- 📊 **变更**: +3 / -1

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+2/-1)
- `.github/workflows/docker_hub.yaml` (+1/-0)

#### 7. 1.4.8 Playwright

- 📅 **日期**: 2025-11-10
- 👤 **作者**: RACH
- 🔗 **提交**: `5d154553`
- 📊 **变更**: +47 / -47

**修改的文件**:

- `.dockerignore` (+6/-1)
- `Dockerfile` (+11/-12)
- `apis/mps.py` (+4/-2)
- `driver/playwright_driver.py` (+13/-30)
- `requirements.txt` (+13/-2)

---

## 🔧 导出功能

**功能描述**: 增强内容导出功能，支持多种格式（PDF/Word/Markdown/HTML/JSON）

**提交数量**: 8 个

**代码变更**: +239 / -80

### 关键提交详情

#### 1. 1.4.6 修正CSV导出功能，保留BOM头

- 📅 **日期**: 2025-08-25
- 👤 **作者**: EricZhou05
- 🔗 **提交**: `9d295a2b`
- 📊 **变更**: +11 / -10

**修改的文件**:

- `web_ui/src/api/export.ts` (+5/-7)
- `web_ui/src/views/article/ArticleListDesktop.vue` (+6/-3)

#### 2. 1.4.6 新增标签导入导出功能

- 📅 **日期**: 2025-09-02
- 👤 **作者**: EricZhou05
- 🔗 **提交**: `1ea5ad73`
- 📊 **变更**: +61 / -6

**修改的文件**:

- `apis/export.py` (+38/-5)
- `web_ui/src/api/export.ts` (+4/-0)
- `web_ui/src/views/TagList.vue` (+19/-1)

#### 3. 1.4.6 增加标签导入、导出功能

- 📅 **日期**: 2025-09-08
- 👤 **作者**: t@123654
- 🔗 **提交**: `3213ce62`
- 📊 **变更**: +44 / -26

**修改的文件**:

- `.gitignore` (+2/-0)
- `apis/message_task.py` (+2/-1)
- `core/config.py` (+6/-5)
- `core/models/base.py` (+1/-1)
- `core/models/config_management.py` (+1/-3)
- `core/models/message_task.py` (+1/-3)
- `core/models/message_task_log.py` (+22/-0)
- `core/models/tags.py` (+1/-3)
- _(还有 11 个文件)_

#### 4. 1.4.7 增加导出md/pdf/html/json/docx功能

- 📅 **日期**: 2025-10-18
- 👤 **作者**: t@123654
- 🔗 **提交**: `8e8d5bd2`
- 📊 **变更**: +12 / -12

**修改的文件**:

- `static/assets/{SysInfo.6836b78e.js => SysInfo.54056797.js}` (+1/-1)
- `static/assets/{TagForm.7a0fed24.js => TagForm.c8dfd7c9.js}` (+1/-1)
- `static/assets/{TagList.30dc75fb.js => TagList.32d3e803.js}` (+1/-1)
- `static/assets/{index.41999601.css => index.e5557f82.css}` (+1/-1)
- `.../assets/{tagManagement.2fb0a6cb.js => tagManagement.66ef3308.js}` (+1/-1)
- `static/index.html` (+2/-2)
- `web_ui/build.bat` (+3/-3)
- `web_ui/dist/index.html` (+2/-2)

#### 5. 1.4.7 增加pdf/docx/json/md导出纪录

- 📅 **日期**: 2025-10-21
- 👤 **作者**: t@123654
- 🔗 **提交**: `4da7b102`
- 📊 **变更**: +51 / -9

**修改的文件**:

- `apis/tools.py` (+9/-2)
- `tools/mdtools/export.py` (+1/-0)
- `web.py` (+1/-0)
- `web_ui/build.bat` (+1/-1)
- `web_ui/dist/index.html` (+1/-1)
- `web_ui/package.json` (+1/-1)
- `web_ui/src/api/tools.ts` (+2/-1)
- `web_ui/src/components/ExportModal.vue` (+3/-1)
- _(还有 7 个文件)_

#### 6. 1.4.7 增加导出md/pdf/html/json/docx功能

- 📅 **日期**: 2025-10-21
- 👤 **作者**: t@123654
- 🔗 **提交**: `03f488d0`
- 📊 **变更**: +1 / -1

**修改的文件**:

- `web.py` (+1/-1)

#### 7. 1.4.7 Fix导出纪录不显示

- 📅 **日期**: 2025-10-21
- 👤 **作者**: t@123654
- 🔗 **提交**: `53c0f5cf`
- 📊 **变更**: +14 / -8

**修改的文件**:

- `apis/tools.py` (+14/-8)

#### 8. 1.4.7 优化部分公众号样式导致导出pdf/docx格式错乱

- 📅 **日期**: 2025-10-21
- 👤 **作者**: t@123654
- 🔗 **提交**: `fdfddb11`
- 📊 **变更**: +45 / -8

**修改的文件**:

- `apis/tools.py` (+2/-1)
- `core/content_format.py` (+33/-5)
- `test_article.py` (+2/-1)
- `tools/mdtools/export.py` (+8/-1)

---

## 🔧 标签管理

**功能描述**: 标签系统的各项改进，包括导入导出、自定义LOGO、预览等

**提交数量**: 17 个

**代码变更**: +726 / -297

### 关键提交详情

#### 1. 1.4.6 标签管理增加自定义LOGO

- 📅 **日期**: 2025-08-26
- 👤 **作者**: t@123654
- 🔗 **提交**: `6874c1af`
- 📊 **变更**: +38 / -19

**修改的文件**:

- `apis/rss.py` (+1/-1)
- `apis/user.py` (+21/-1)
- `driver/token.py` (+1/-2)
- `.../{SysInfo.00fcfa52.js => SysInfo.4a3bb14b.js}` (+1/-1)
- `static/assets/TagForm.096307b7.js` (+1/-0)
- `static/assets/TagForm.b3c0280e.js` (+0/-1)
- `static/assets/TagForm.cc501652.css` (+1/-0)
- `static/assets/TagForm.f2399f47.css` (+0/-1)
- _(还有 8 个文件)_

#### 2. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-22
- 👤 **作者**: RachelOS
- 🔗 **提交**: `f5195673`
- 📊 **变更**: +52 / -75

**修改的文件**:

- `core/lax/template_parser.py` (+14/-2)
- `public/templates/article_detail.html` (+5/-0)
- `public/templates/articles.html` (+6/-0)
- `public/templates/home.html` (+3/-0)
- `.../templates/includes/article_detail_styles.html` (+1/-0)
- `public/templates/includes/articles_styles.html` (+2/-0)
- `public/templates/includes/empty_state.html` (+1/-0)
- `public/templates/includes/footer.html` (+1/-0)
- _(还有 15 个文件)_

#### 3. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-23
- 👤 **作者**: RachelOS
- 🔗 **提交**: `729af552`
- 📊 **变更**: +83 / -24

**修改的文件**:

- `driver/wxarticle.py` (+14/-0)
- `public/templates/article_detail.html` (+2/-3)
- `public/templates/articles.html` (+0/-2)
- `public/templates/home.html` (+2/-2)
- `.../templates/includes/article_detail_styles.html` (+5/-0)
- `public/templates/includes/articles_styles.html` (+7/-2)
- `public/templates/includes/footer.html` (+7/-0)
- `public/templates/includes/header.html` (+17/-4)
- _(还有 4 个文件)_

#### 4. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-23
- 👤 **作者**: RachelOS
- 🔗 **提交**: `40297a28`
- 📊 **变更**: +2 / -1

**修改的文件**:

- `ReadMe.md` (+2/-1)

#### 5. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-23
- 👤 **作者**: RachelOS
- 🔗 **提交**: `50129b65`
- 📊 **变更**: +2 / -0

**修改的文件**:

- `ReadMe.md` (+1/-0)
- `views/home.py` (+1/-0)

#### 6. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-23
- 👤 **作者**: RachelOS
- 🔗 **提交**: `ad0375c0`
- 📊 **变更**: +126 / -0

**修改的文件**:

- `apis/article.py` (+4/-0)
- `apis/cache.py` (+17/-0)
- `apis/tags.py` (+6/-0)
- `config.example.yaml` (+4/-0)
- `core/cache.py` (+52/-0)
- `docs/view-cache.md` (+41/-0)
- `views/articles.py` (+1/-0)
- `views/home.py` (+1/-0)

#### 7. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-23
- 👤 **作者**: RachelOS
- 🔗 **提交**: `12384113`
- 📊 **变更**: +64 / -49

**修改的文件**:

- `core/config.py` (+1/-1)
- `public/templates/article_detail.html` (+1/-1)
- `public/templates/articles.html` (+6/-2)
- `views/__init__.py` (+1/-1)
- `views/articles.py` (+21/-14)
- `views/home.py` (+0/-30)
- `views/tags.py` (+34/-0)

#### 8. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-23
- 👤 **作者**: RachelOS
- 🔗 **提交**: `31046614`
- 📊 **变更**: +0 / -2

**修改的文件**:

- `ReadMe.md` (+0/-2)

#### 9. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `111253b2`
- 📊 **变更**: +31 / -18

**修改的文件**:

- `apis/sys_info.py` (+1/-2)
- `core/article_lax.py` (+17/-5)
- `core/cache.py` (+2/-3)
- `public/templates/article_detail.html` (+1/-2)
- `public/templates/home.html` (+6/-4)
- `.../templates/includes/article_detail_styles.html` (+2/-0)
- `public/templates/includes/footer.html` (+1/-1)
- `public/templates/includes/header.html` (+1/-1)

#### 10. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `93e15343`
- 📊 **变更**: +113 / -4

**修改的文件**:

- `core/lax/template_parser.py` (+22/-0)
- `public/templates/home.html` (+2/-2)
- `public/templates/includes/header.html` (+1/-0)
- `public/templates/mps.html` (+10/-0)
- `public/templates/tags.html` (+10/-0)
- `views/__init__.py` (+1/-1)
- `views/config.py` (+1/-1)
- `views/mps.py` (+34/-0)
- _(还有 1 个文件)_

#### 11. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `3c469882`
- 📊 **变更**: +6 / -8

**修改的文件**:

- `public/templates/includes/header.html` (+1/-0)
- `public/templates/mps.html` (+1/-1)
- `views/articles.py` (+2/-5)
- `views/mps.py` (+2/-2)

#### 12. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `7817470a`
- 📊 **变更**: +21 / -17

**修改的文件**:

- `public/templates/home.html` (+1/-1)
- `public/templates/includes/breadcrumb.html` (+12/-0)
- `public/templates/includes/header.html` (+3/-4)
- `public/templates/mps.html` (+4/-9)
- `public/templates/tags.html` (+1/-3)

#### 13. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `6675f4f6`
- 📊 **变更**: +24 / -14

**修改的文件**:

- `core/lax/template_parser_optimization_notes.md` (+12/-0)
- `views/articles.py` (+12/-13)
- `views/home.py` (+0/-1)

#### 14. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `b85c76fa`
- 📊 **变更**: +58 / -38

**修改的文件**:

- `public/templates/home.html` (+3/-3)
- `public/templates/includes/breadcrumb.html` (+1/-1)
- `public/templates/includes/footer.html` (+1/-1)
- `public/templates/includes/header.html` (+3/-1)
- `public/templates/includes/mps.html` (+4/-0)
- `public/templates/includes/tags.html` (+5/-0)
- `public/templates/mps.html` (+1/-4)
- `views/articles.py` (+4/-1)
- _(还有 5 个文件)_

#### 15. 1.4.8-增加标签预览

- 📅 **日期**: 2025-12-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `9e5953f6`
- 📊 **变更**: +24 / -1

**修改的文件**:

- `web_ui/src/views/article/ArticleListDesktop.vue` (+24/-1)

_...还有 2 个提交未列出_

---

## 🔧 ARM64支持

**功能描述**: 添加 ARM64 架构支持，适配更多硬件平台

**提交数量**: 9 个

**代码变更**: +125 / -52

### 关键提交详情

#### 1. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-22
- 👤 **作者**: t@123654
- 🔗 **提交**: `8fc47de1`
- 📊 **变更**: +64 / -25

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+8/-3)
- `.github/workflows/docker_hub.yaml` (+1/-0)
- `Dockerfiles/base/Dockerfile` (+25/-10)
- `Dockerfiles/py3.13.1/Dockerfile` (+12/-3)
- `test_article.py` (+1/-2)
- `tools/mdtools/md2doc.py` (+17/-7)

#### 2. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-22
- 👤 **作者**: t@123654
- 🔗 **提交**: `44e73d3d`
- 📊 **变更**: +4 / -0

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+4/-0)

#### 3. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-22
- 👤 **作者**: t@123654
- 🔗 **提交**: `90fe2a24`
- 📊 **变更**: +2 / -5

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+1/-4)
- `.github/workflows/docker_hub.yaml` (+1/-1)

#### 4. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-22
- 👤 **作者**: t@123654
- 🔗 **提交**: `b9c8f06e`
- 📊 **变更**: +1 / -5

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+1/-5)

#### 5. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-22
- 👤 **作者**: t@123654
- 🔗 **提交**: `7ac6e508`
- 📊 **变更**: +5 / -0

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+5/-0)

#### 6. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-22
- 👤 **作者**: t@123654
- 🔗 **提交**: `69f8b45f`
- 📊 **变更**: +1 / -1

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+1/-1)

#### 7. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-22
- 👤 **作者**: t@123654
- 🔗 **提交**: `258db9ff`
- 📊 **变更**: +1 / -10

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+1/-10)

#### 8. 1.4.7 增加Arm64版本镜像

- 📅 **日期**: 2025-10-23
- 👤 **作者**: t@123654
- 🔗 **提交**: `3f508115`
- 📊 **变更**: +6 / -1

**修改的文件**:

- `ReadMe.md` (+6/-1)

#### 9. 增加Arm64镜像支持

- 📅 **日期**: 2025-10-24
- 👤 **作者**: t@123654
- 🔗 **提交**: `47ffd6e9`
- 📊 **变更**: +41 / -5

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+1/-1)
- `MULTIARCH_BUILD.md` (+34/-0)
- `core/content_format.py` (+1/-1)
- `dock_build.bat` (+5/-2)
- `test_docker.bat` (+0/-1)

---

## 🔧 通知系统

**功能描述**: 浏览器通知功能，及时提醒用户新文章

**提交数量**: 2 个

**代码变更**: +44 / -3

### 关键提交详情

#### 1. feat: add browser notification for new articles

- 📅 **日期**: 2025-12-09
- 👤 **作者**: yangjuntao
- 🔗 **提交**: `30692cbe`
- 📊 **变更**: +39 / -0

**修改的文件**:

- `web_ui/src/utils/browserNotification.ts` (+32/-0)
- `web_ui/src/views/MessageTaskList.vue` (+7/-0)

#### 2. 1.4.8-API方式扫码不发通知修复

- 📅 **日期**: 2025-12-17
- 👤 **作者**: RachelOS
- 🔗 **提交**: `fb4487fb`
- 📊 **变更**: +5 / -3

**修改的文件**:

- `ReadMe.md` (+1/-0)
- `driver/wx_api.py` (+2/-1)
- `test_article.py` (+2/-2)

---

## 🔧 已读功能

**功能描述**: 文章已读状态管理

**提交数量**: 3 个

**代码变更**: +133 / -139

### 关键提交详情

#### 1. 1.4.8-增加已读功能

- 📅 **日期**: 2025-12-18
- 👤 **作者**: RachelOS
- 🔗 **提交**: `94c39a1e`
- 📊 **变更**: +0 / -1

**修改的文件**:

- `ReadMe.md` (+0/-1)

#### 2. 1.4.8-增加已读功能

- 📅 **日期**: 2025-12-18
- 👤 **作者**: RachelOS
- 🔗 **提交**: `7651870a`
- 📊 **变更**: +1 / -134

**修改的文件**:

- `ReadMe.md` (+1/-0)
- `static/assets/SysInfo.2d0e6991.css` (+0/-1)
- `static/assets/SysInfo.490a5766.js` (+0/-2)
- `static/assets/TagForm.cc501652.css` (+0/-1)
- `static/assets/TagForm.efd3891b.js` (+0/-1)
- `static/assets/TagList.951ef3a5.css` (+0/-1)
- `static/assets/TagList.b5fafeb2.js` (+0/-1)
- `static/assets/abap.4bb81009.js` (+0/-1)
- _(还有 92 个文件)_

#### 3. 1.4.8-增加已读功能

- 📅 **日期**: 2025-12-18
- 👤 **作者**: RachelOS
- 🔗 **提交**: `5e011975`
- 📊 **变更**: +132 / -4

**修改的文件**:

- `ReadMe.md` (+1/-1)
- `static/assets/SysInfo.2d0e6991.css` (+1/-0)
- `static/assets/SysInfo.490a5766.js` (+2/-0)
- `static/assets/TagForm.cc501652.css` (+1/-0)
- `static/assets/TagForm.efd3891b.js` (+1/-0)
- `static/assets/TagList.951ef3a5.css` (+1/-0)
- `static/assets/TagList.b5fafeb2.js` (+1/-0)
- `static/assets/abap.4bb81009.js` (+1/-0)
- _(还有 92 个文件)_

---

## 🔧 API扫码登录

**功能描述**: API方式扫码登录优化，改善用户体验

**提交数量**: 2 个

**代码变更**: +88 / -113

### 关键提交详情

#### 1. "1.4.7 增加API方式扫码"

- 📅 **日期**: 2025-11-06
- 👤 **作者**: RACH
- 🔗 **提交**: `8d248e74`
- 📊 **变更**: +48 / -105

**修改的文件**:

- `.wdm/drivers.json` (+0/-1)
- `Dockerfiles/base-mini/Dockerfile` (+3/-0)
- `apis/auth.py` (+1/-1)
- `build.bat` (+0/-6)
- `dock_build.bat` (+1/-1)
- `driver/base.py` (+1/-1)
- `driver/cookies.py` (+1/-1)
- `driver/firefox_driver.py.del` (+0/-33)
- _(还有 12 个文件)_

#### 2. 1.4.8-API方式扫码多线程优化

- 📅 **日期**: 2025-12-17
- 👤 **作者**: RachelOS
- 🔗 **提交**: `792faeed`
- 📊 **变更**: +40 / -8

**修改的文件**:

- `ReadMe.md` (+2/-1)
- `driver/wx.py` (+2/-2)
- `driver/wx_api.py` (+36/-5)

---

## 🔧 任务调度

**功能描述**: 优化任务调度和采集频率，提升稳定性

**提交数量**: 5 个

**代码变更**: +111 / -50

### 关键提交详情

#### 1. 1.4.6 修复前端Cron星期定义与后端APScheduler不一致问题 更改原因: Cron星期定义（0=周日）与底层APScheduler（0=周一）不一致。 更改方法: 内部自动转换星期字段的值。

- 📅 **日期**: 2025-09-19
- 👤 **作者**: EricZhou05
- 🔗 **提交**: `3fe9235e`
- 📊 **变更**: +34 / -15

**修改的文件**:

- `core/task/task.py` (+34/-15)

#### 2. 1.4.8-优化采集间隔

- 📅 **日期**: 2025-12-18
- 👤 **作者**: RachelOS
- 🔗 **提交**: `205b909b`
- 📊 **变更**: +54 / -20

**修改的文件**:

- `check_pk.py` (+0/-7)
- `config.example.yaml` (+1/-1)
- `core/wx/base.py` (+11/-1)
- `core/wx/model/web.py` (+1/-1)
- `driver/playwright_driver.py` (+2/-1)
- `driver/wxarticle.py` (+5/-6)
- `jobs/fetch_no_article.py` (+7/-1)
- `main.py` (+2/-0)
- _(还有 2 个文件)_

#### 3. 1.4.8-优化采集频度

- 📅 **日期**: 2025-12-18
- 👤 **作者**: RachelOS
- 🔗 **提交**: `f42241b6`
- 📊 **变更**: +7 / -5

**修改的文件**:

- `core/wx/base.py` (+1/-2)
- `driver/wxarticle.py` (+6/-3)

#### 4. 1.4.8-优化获取内容间隔，降低被风控概率

- 📅 **日期**: 2025-12-18
- 👤 **作者**: RachelOS
- 🔗 **提交**: `b7dceccd`
- 📊 **变更**: +15 / -10

**修改的文件**:

- `core/wait.py` (+7/-0)
- `core/wx/base.py` (+4/-3)
- `driver/wxarticle.py` (+2/-5)
- `jobs/fetch_no_article.py` (+2/-2)

#### 5. 1.4.8-优化获取内容间隔，降低被风控概率

- 📅 **日期**: 2025-12-18
- 👤 **作者**: RachelOS
- 🔗 **提交**: `d8f3887c`
- 📊 **变更**: +1 / -0

**修改的文件**:

- `ReadMe.md` (+1/-0)

---

## 🔧 安全性

**功能描述**: 安全性增强，包括CSRF防护和安全漏洞修复

**提交数量**: 4 个

**代码变更**: +41 / -29

### 关键提交详情

#### 1. 1.4.6 CSRF检验

- 📅 **日期**: 2025-08-29
- 👤 **作者**: t@123654
- 🔗 **提交**: `2f06d8e0`
- 📊 **变更**: +14 / -12

**修改的文件**:

- `core/wx/base.py` (+0/-2)
- `core/wx/wx1.py` (+2/-1)
- `core/wx/wx2.py` (+2/-1)
- `core/wx/wx3.py` (+2/-1)
- `publish.bat` (+1/-0)
- `static/assets/{SysInfo.4a3bb14b.js => SysInfo.74dfa5b3.js}` (+1/-1)
- `static/assets/{TagForm.096307b7.js => TagForm.e7dc5b41.js}` (+1/-1)
- `static/assets/{TagList.651f6f2a.js => TagList.220e6fd1.js}` (+1/-1)
- _(还有 4 个文件)_

#### 2. Potential fix for code scanning alert no. 131: Uncontrolled data used in path expression

- 📅 **日期**: 2025-10-21
- 👤 **作者**: Rachel
- 🔗 **提交**: `e5c3e8ba`
- 📊 **变更**: +10 / -11

**修改的文件**:

- `apis/tools.py` (+10/-11)

#### 3. Potential fix for code scanning alert no. 129: Uncontrolled data used in path expression

- 📅 **日期**: 2025-10-21
- 👤 **作者**: Rachel
- 🔗 **提交**: `719dd4c8`
- 📊 **变更**: +15 / -6

**修改的文件**:

- `apis/tools.py` (+15/-6)

#### 4. Potential fix for code scanning alert no. 141: Workflow does not contain permissions

- 📅 **日期**: 2025-10-25
- 👤 **作者**: Rachel
- 🔗 **提交**: `f727fa07`
- 📊 **变更**: +2 / -0

**修改的文件**:

- `.github/workflows/docker-publish.yaml` (+2/-0)

---

## 🔧 UI优化

**功能描述**: 用户界面改进和视觉优化

**提交数量**: 2 个

**代码变更**: +17 / -7

### 关键提交详情

#### 1. 1.4.6 增加下拉栏三角图标的动画

- 📅 **日期**: 2025-08-28
- 👤 **作者**: EricZhou05
- 🔗 **提交**: `0bcfd1d9`
- 📊 **变更**: +9 / -0

**修改的文件**:

- `web_ui/src/views/article/ArticleListDesktop.vue` (+9/-0)

#### 2. 1.4.7 UI更新

- 📅 **日期**: 2025-10-21
- 👤 **作者**: t@123654
- 🔗 **提交**: `3f68f160`
- 📊 **变更**: +8 / -7

**修改的文件**:

- `static/assets/{SysInfo.54056797.js => SysInfo.a20c8e5a.js}` (+1/-1)
- `static/assets/{TagForm.c8dfd7c9.js => TagForm.d6adf05f.js}` (+1/-1)
- `static/assets/{TagList.32d3e803.js => TagList.175bcb71.js}` (+1/-1)
- `static/assets/index.e5557f82.css` (+0/-1)
- `static/assets/index.f3e9b600.css` (+1/-0)
- `.../assets/{tagManagement.66ef3308.js => tagManagement.dc97cdc1.js}` (+1/-1)
- `static/index.html` (+2/-2)
- `web_ui/build.bat` (+1/-0)

---

## 🔧 文档

**功能描述**: 项目文档更新和补充

**提交数量**: 6 个

**代码变更**: +109 / -40

### 关键提交详情

#### 1. 1.4.7 添加项目原理

- 📅 **日期**: 2025-10-28
- 👤 **作者**: t@123654
- 🔗 **提交**: `41a38fab`
- 📊 **变更**: +22 / -2

**修改的文件**:

- `ReadMe.md` (+1/-0)
- `...11\215\347\253\257\346\236\266\346\236\204.png"` (+0/-1)
- `...36\266\346\236\204\345\216\237\347\220\206.png"` (+0/-1)
- `driver/wx_api.py` (+21/-0)

#### 2. 1.4.7 添加项目原理

- 📅 **日期**: 2025-10-28
- 👤 **作者**: t@123654
- 🔗 **提交**: `28bc07cd`
- 📊 **变更**: +1 / -1

**修改的文件**:

- `ReadMe.md` (+1/-1)

#### 3. 1.4.7 添加项目原理

- 📅 **日期**: 2025-10-28
- 👤 **作者**: t@123654
- 🔗 **提交**: `fc98f9ae`
- 📊 **变更**: +80 / -35

**修改的文件**:

- `README-CN.md` (+56/-0)
- `ReadMe.md` (+24/-35)

#### 4. 1.4.7 添加项目原理

- 📅 **日期**: 2025-10-28
- 👤 **作者**: t@123654
- 🔗 **提交**: `4f402a83`
- 📊 **变更**: +4 / -0

**修改的文件**:

- `README-CN.md` (+2/-0)
- `ReadMe.md` (+2/-0)

#### 5. 1.4.7 添加项目原理

- 📅 **日期**: 2025-10-28
- 👤 **作者**: t@123654
- 🔗 **提交**: `52092c3d`
- 📊 **变更**: +0 / -0

**修改的文件**:


#### 6. 1.4.7 添加项目原理

- 📅 **日期**: 2025-10-28
- 👤 **作者**: t@123654
- 🔗 **提交**: `6ff01582`
- 📊 **变更**: +2 / -2

**修改的文件**:

- `README.zh-CN.md` (+1/-1)
- `ReadMe.md` (+1/-1)

---

## 🔧 性能优化

**功能描述**: 系统性能优化和资源管理

**提交数量**: 4 个

**代码变更**: +227 / -24

### 关键提交详情

#### 1. 1.4.6 任务缓存问题，解决新任务不更新

- 📅 **日期**: 2025-09-04
- 👤 **作者**: t@123654
- 🔗 **提交**: `d5e5962d`
- 📊 **变更**: +6 / -2

**修改的文件**:

- `core/db.py` (+1/-1)
- `driver/token.py` (+2/-0)
- `jobs/article.py` (+1/-1)
- `jobs/taskmsg.py` (+2/-0)

#### 2. 1.4.8-资源占用溢出修复

- 📅 **日期**: 2025-12-22
- 👤 **作者**: RachelOS
- 🔗 **提交**: `7f03eca1`
- 📊 **变更**: +23 / -17

**修改的文件**:

- `ReadMe.md` (+1/-1)
- `driver/auth.py` (+4/-1)
- `driver/playwright_driver.py` (+2/-3)
- `driver/wx.py` (+8/-8)
- `job.py` (+1/-0)
- `jobs/mps.py` (+0/-1)
- `test_article.py` (+7/-3)

#### 3. 1.4.8-资源占用溢出修复

- 📅 **日期**: 2025-12-22
- 👤 **作者**: RachelOS
- 🔗 **提交**: `e8034bbe`
- 📊 **变更**: +198 / -4

**修改的文件**:

- `Dockerfile` (+0/-1)
- `docs/cache-config.md` (+13/-0)
- `driver/auth.py` (+1/-1)
- `driver/playwright_driver.py` (+1/-1)
- `test_article.py` (+1/-1)
- `views/INSTALL.md` (+24/-0)
- `views/README.md` (+16/-0)
- `views/__init__.py` (+2/-0)
- _(还有 7 个文件)_

#### 4. 1.4.8-资源占用溢出修复

- 📅 **日期**: 2025-12-22
- 👤 **作者**: RachelOS
- 🔗 **提交**: `3adaa0ee`
- 📊 **变更**: +0 / -1

**修改的文件**:

- `ReadMe.md` (+0/-1)

---

## 🔧 Bug修复

**功能描述**: 各类问题修复和功能完善

**提交数量**: 55 个

**代码变更**: +3123 / -566

### 关键提交详情

#### 1. fix: add rfc822 timezone in rss result

- 📅 **日期**: 2025-10-15
- 👤 **作者**: TianKai Ma
- 🔗 **提交**: `7a4c9d5b`
- 📊 **变更**: +39 / -10

**修改的文件**:

- `apis/rss.py` (+7/-3)
- `core/rss.py` (+32/-7)

#### 2. 修复linux环境下由于文件大小写问题导致的无法正常加载页面

- 📅 **日期**: 2025-10-31
- 👤 **作者**: unfazed
- 🔗 **提交**: `39d6067a`
- 📊 **变更**: +2 / -2

**修改的文件**:

- `web_ui/src/App.vue` (+2/-2)

#### 3. 修复部分公众号不能添加订阅的问题

- 📅 **日期**: 2025-10-31
- 👤 **作者**: unfazed
- 🔗 **提交**: `7025d3a4`
- 📊 **变更**: +27 / -8

**修改的文件**:

- `driver/wxarticle.py` (+27/-8)

#### 4. 1.4.8 "Fix"

- 📅 **日期**: 2025-11-09
- 👤 **作者**: RACH
- 🔗 **提交**: `3a4e0b9a`
- 📊 **变更**: +26 / -46

**修改的文件**:

- `publish.bat` (+1/-1)
- `static/assets/SysInfo.b2fa594f.js` (+0/-3)
- `static/assets/SysInfo.cbaf9294.js` (+3/-0)
- `.../{TagForm.3c8acb94.js => TagForm.e212e365.js}` (+1/-1)
- `.../{TagList.7e7cc5be.js => TagList.dd2479c0.js}` (+1/-1)
- `.../{cssMode.40d36965.js => cssMode.fb957910.js}` (+1/-1)
- `...marker2.3f56eac0.js => freemarker2.eca5ebc9.js}` (+1/-1)
- `...ndlebars.46cbb6ce.js => handlebars.c29b9016.js}` (+1/-1)
- _(还有 18 个文件)_

#### 5. 1.4.8 Fix

- 📅 **日期**: 2025-11-09
- 👤 **作者**: RACH
- 🔗 **提交**: `7b528a2c`
- 📊 **变更**: +5 / -4

**修改的文件**:

- `driver/playwright_driver.py` (+4/-3)
- `publish.bat` (+1/-1)

#### 6. '1.4.8 修复通过文章添加订阅'

- 📅 **日期**: 2025-11-10
- 👤 **作者**: RACH
- 🔗 **提交**: `995125de`
- 📊 **变更**: +30 / -23

**修改的文件**:

- `apis/mps.py` (+2/-1)
- `driver/playwright_driver.py` (+23/-21)
- `driver/wxarticle.py` (+2/-0)
- `test_article.py` (+3/-1)

#### 7. 1.4.8 Fix

- 📅 **日期**: 2025-11-17
- 👤 **作者**: RACH
- 🔗 **提交**: `974bbcd3`
- 📊 **变更**: +1901 / -8

**修改的文件**:

- `apis/mps.py` (+1/-1)
- `core/wx/base.py` (+1/-1)
- `driver/playwright_driver.py` (+1/-1)
- `driver/wx_api.py` (+1/-1)
- `driver/wxarticle.py` (+1/-1)
- `qtserver/README-TEST.md` (+1/-0)
- `qtserver/README.md` (+1/-0)
- `qtserver/mqtt-client-test.js` (+2/-0)
- _(还有 1484 个文件)_

#### 8. 1.4.8 Fix

- 📅 **日期**: 2025-11-17
- 👤 **作者**: RACH
- 🔗 **提交**: `2bf058f8`
- 📊 **变更**: +1 / -0

**修改的文件**:

- `qtserver/.gitignore` (+1/-0)

#### 9. Fix

- 📅 **日期**: 2025-11-24
- 👤 **作者**: RachelOS
- 🔗 **提交**: `14d692cd`
- 📊 **变更**: +77 / -29

**修改的文件**:

- `.dockerignore` (+1/-0)
- `.github/workflows/docker-publish.yaml` (+1/-0)
- `.github/workflows/docker_hub.yaml` (+1/-0)
- `Dockerfile` (+1/-1)
- `Dockerfiles/base-mini/Dockerfile` (+1/-1)
- `config.example.yaml` (+1/-1)
- `daemon.json` (+0/-1)
- `dock_build.bat` (+1/-1)
- _(还有 1838 个文件)_

#### 10. FIx

- 📅 **日期**: 2025-11-26
- 👤 **作者**: RachelOS
- 🔗 **提交**: `cf015e1b`
- 📊 **变更**: +4 / -4

**修改的文件**:

- `Dockerfile` (+2/-2)
- `Dockerfiles/base-mini/Dockerfile` (+1/-1)
- `driver/wxarticle.py` (+1/-1)

_...还有 45 个提交未列出_

---

## 🔧 其他

**功能描述**: 其他更新和改进

**提交数量**: 20 个

**代码变更**: +766 / -595

### 关键提交详情

#### 1. 1.4.6 1.4.6

- 📅 **日期**: 2025-09-19
- 👤 **作者**: t@123654
- 🔗 **提交**: `ccf63186`
- 📊 **变更**: +39 / -24

**修改的文件**:

- `Dockerfiles/base/Dockerfile` (+1/-0)
- `Dockerfiles/py3.13.1/Dockerfile` (+0/-1)
- `ReadMe.md` (+1/-0)
- `core/config.py` (+1/-0)
- `dock_build.bat` (+1/-1)
- `driver/wx.py` (+1/-1)
- `start.sh` (+1/-0)
- `test_article.py` (+1/-1)
- _(还有 8 个文件)_

#### 2. 1.4.7 1.4.7

- 📅 **日期**: 2025-10-18
- 👤 **作者**: t@123654
- 🔗 **提交**: `82d9c8f1`
- 📊 **变更**: +63 / -11

**修改的文件**:

- `.gitignore` (+1/-1)
- `Dockerfile` (+1/-1)
- `Dockerfiles/py3.13.1/Dockerfile` (+1/-0)
- `apis/message_task.py` (+1/-0)
- `apis/tools.py` (+6/-0)
- `apis/user.py` (+1/-1)
- `core/common/file_tools.py` (+1/-0)
- `core/content_format.py` (+1/-1)
- _(还有 16 个文件)_

#### 3. -消息任务增加编辑器、消息任务模板解析引擎调整去除多余,号

- 📅 **日期**: 2025-10-25
- 👤 **作者**: t@123654
- 🔗 **提交**: `4c175696`
- 📊 **变更**: +174 / -67

**修改的文件**:

- `.vscode/settings.json` (+1/-0)
- `CODE_OF_CONDUCT.md` (+0/-8)
- `MULTIARCH_BUILD.md` (+0/-11)
- `core/lax/template_example.txt` (+1/-2)
- `core/lax/template_parser.py` (+1/-2)
- `core/lax/template_test_cases.txt` (+6/-0)
- `core/lax/test_template_parser.py` (+7/-0)
- `debug_template_parser.py` (+1/-1)
- _(还有 108 个文件)_

#### 4. Finish frontend-blank-on-load

- 📅 **日期**: 2025-10-31
- 👤 **作者**: unfazed
- 🔗 **提交**: `aa69571c`
- 📊 **变更**: +0 / -0

#### 5. 1.4.7 1.4.7

- 📅 **日期**: 2025-11-01
- 👤 **作者**: RachelOS
- 🔗 **提交**: `31ecdf0a`
- 📊 **变更**: +53 / -13

**修改的文件**:

- `apis/auth.py` (+1/-1)
- `driver/cookies.py` (+1/-1)
- `driver/token.py` (+1/-1)
- `driver/wx_api.py` (+45/-8)
- `test_article.py` (+4/-1)
- `web_ui/src/App.vue` (+1/-1)

#### 6. 1.4.7 1.4.7

- 📅 **日期**: 2025-11-04
- 👤 **作者**: RachelOs
- 🔗 **提交**: `f151d1e3`
- 📊 **变更**: +205 / -200

**修改的文件**:

- `.github/ISSUE_TEMPLATE/bug_report.md` (+1/-1)
- `.github/ISSUE_TEMPLATE/custom.md` (+1/-1)
- `.github/ISSUE_TEMPLATE/feature_request.md` (+1/-1)
- `.github/workflows/base_os.yaml` (+1/-1)
- `.github/workflows/buidweb.yaml` (+1/-1)
- `.github/workflows/docker-publish.yaml` (+1/-1)
- `.github/workflows/docker_hub.yaml` (+1/-1)
- `.github/workflows/issues.yaml` (+1/-1)
- _(还有 345 个文件)_

#### 7. 1.4.7 1.4.7

- 📅 **日期**: 2025-11-04
- 👤 **作者**: RachelOs
- 🔗 **提交**: `30eee6fe`
- 📊 **变更**: +0 / -0

#### 8. 1.4.7 1.4.7

- 📅 **日期**: 2025-11-04
- 👤 **作者**: RACH
- 🔗 **提交**: `f3c6bd2f`
- 📊 **变更**: +1 / -0

**修改的文件**:

- `requirements.txt` (+1/-0)

#### 9. 1.4.7 1.4.7

- 📅 **日期**: 2025-11-04
- 👤 **作者**: RACH
- 🔗 **提交**: `bc0fdf64`
- 📊 **变更**: +26 / -26

**修改的文件**:

- `driver/wxarticle.py` (+26/-26)

#### 10. "1.4.7 "仓库版本冲突wxarticle.py""

- 📅 **日期**: 2025-11-04
- 👤 **作者**: RACH
- 🔗 **提交**: `0cf5b048`
- 📊 **变更**: +3 / -47

**修改的文件**:

- `.wdm/drivers.json` (+1/-0)
- `dock_build.bat` (+1/-0)
- `driver/.wdm/drivers.json` (+0/-1)
- `driver/wxarticle.py` (+1/-46)

#### 11. 1.4.8 1.4.8

- 📅 **日期**: 2025-11-07
- 👤 **作者**: RACH
- 🔗 **提交**: `3c5f36c9`
- 📊 **变更**: +42 / -75

**修改的文件**:

- `.dockerignore` (+4/-0)
- `.github/workflows/docker-publish.yaml` (+2/-3)
- `.github/workflows/docker_hub.yaml` (+4/-2)
- `Dockerfile` (+1/-1)
- `README.zh-CN.md` (+1/-0)
- `config.example.yaml` (+3/-1)
- `core/ver.py` (+1/-1)
- `core/wx/cfg.py` (+2/-1)
- _(还有 6 个文件)_

#### 12. 1.4.8 1.4.8

- 📅 **日期**: 2025-11-07
- 👤 **作者**: RACH
- 🔗 **提交**: `e0ea7e8a`
- 📊 **变更**: +1 / -1

**修改的文件**:

- `.github/workflows/release.yaml` (+1/-1)

#### 13. 1.4.8 1.4.8

- 📅 **日期**: 2025-11-07
- 👤 **作者**: RACH
- 🔗 **提交**: `0698f041`
- 📊 **变更**: +0 / -1

**修改的文件**:

- `test_article.py` (+0/-1)

#### 14. 1.4.8 1.4.8

- 📅 **日期**: 2025-11-08
- 👤 **作者**: RACH
- 🔗 **提交**: `cc728353`
- 📊 **变更**: +37 / -12

**修改的文件**:

- `dock_build.bat` (+2/-2)
- `driver/playwright_driver.py` (+35/-10)

#### 15. 修改提示音

- 📅 **日期**: 2025-12-10
- 👤 **作者**: yangjuntao
- 🔗 **提交**: `1b7b4b2d`
- 📊 **变更**: +1 / -1

**修改的文件**:

- `web_ui/src/utils/browserNotification.ts` (+1/-1)

_...还有 5 个提交未列出_

---

## 📊 统计信息

### 功能分类统计

| 分类 | 提交数 | 代码变更 | 占比 |
| --- | --- | --- | --- |
| Bug修复 | 55 | +3123/-566 | 37.2% |
| 其他 | 20 | +766/-595 | 13.5% |
| 标签管理 | 17 | +726/-297 | 11.5% |
| ARM64支持 | 9 | +125/-52 | 6.1% |
| 导出功能 | 8 | +239/-80 | 5.4% |
| 浏览器引擎升级 | 7 | +141/-97 | 4.7% |
| 文档 | 6 | +109/-40 | 4.1% |
| 任务调度 | 5 | +111/-50 | 3.4% |
| PostgreSQL支持 | 4 | +71/-78 | 2.7% |
| 安全性 | 4 | +41/-29 | 2.7% |
| 性能优化 | 4 | +227/-24 | 2.7% |
| 已读功能 | 3 | +133/-139 | 2.0% |
| 通知系统 | 2 | +44/-3 | 1.4% |
| API扫码登录 | 2 | +88/-113 | 1.4% |
| UI优化 | 2 | +17/-7 | 1.4% |

### 贡献者统计

| 贡献者 | 提交数 | 代码变更 |
| --- | --- | --- |
| RachelOS | 79 | +2428/-1078 |
| t@123654 | 32 | +814/-376 |
| RACH | 20 | +2262/-445 |
| EricZhou05 | 4 | +115/-31 |
| Rachel | 4 | +28/-18 |
| unfazed | 3 | +29/-10 |
| RachelOs | 2 | +205/-200 |
| yangjuntao | 2 | +40/-1 |
| TianKai Ma | 1 | +39/-10 |
| dependabot[bot] | 1 | +1/-1 |

### 月度活跃度

| 月份 | 提交数 |
| --- | --- |
| 2025-08 | 4 |
| 2025-09 | 5 |
| 2025-10 | 34 |
| 2025-11 | 35 |
| 2025-12 | 67 |
| 2026-01 | 3 |

---

## 📝 总结

本次版本迭代（1.4.6 → 1.4.8）历时约5个月，包含了:

- **167** 个提交
- **+5961** 行代码新增
- **-2170** 行代码删除

主要实现了数据库扩展、浏览器引擎升级、多格式导出、ARM64支持等重要功能，
同时进行了大量的bug修复和性能优化，显著提升了系统的稳定性和易用性。

---

*此文档由自动化工具生成于 2026-01-19*
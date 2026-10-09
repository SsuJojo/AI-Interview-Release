# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/).

## [Unreleased]

_No unreleased changes yet._

## [v1.0.64]

### Added

- add Cloudflare Worker proxying release downloads to GitHub

### Fixed

- 按审查意见加固会话对账的并发与判据
- 面试会话恢复时与服务端对账，避免误报提交失败
- 收紧注册判重，用户名与邮箱各查各的字段

## [v1.0.63]

### Fixed

- stop double-dedenting release notes heredoc body

## [v1.0.62]

### Added

- add i18n coverage for remaining UI pages

### Fixed

- remove narrow-screen text clipping on profile, room and resume
- stop hiding download entry in Electron-based IDE previews
- prevent English text overflow on nav, hero and cards

## [v1.0.61]

### Added

- add admin management console

### Fixed

- improve release metadata generation

## [v1.0.60]

### Fixed

- don't force resume upload when opening My page

## [v1.0.59]

### Fixed

- filter download release assets

## [v1.0.58]

### Fixed

- normalize configured resume extensions

### Security

- bound resume upload and parsing resources
- enforce configured origin allowlist
- add explicit origin allowlist parser

## [v1.0.57]

### Added

- call cached resume session endpoint
- expose cached resume session endpoint
- create sessions from saved resumes
- define cached resume session request
- persist resumes for cached job sessions

### Fixed

- start cached jobs in fresh sessions

## [v1.0.56]

### Fixed

- localize API errors and network fallbacks

## [v1.0.55]

### Fixed

- prevent navigation after renaming interview records

## [v1.0.54]

### Fixed

- remove demo data fallbacks

## [v1.0.53]

### Fixed

- render report summary in report view
- render real analysis summary

## [v1.0.52]

### Fixed

- preserve speech draft when recognition stops

## [v1.0.51]

### Fixed

- clear stale user state on expiry
- log out expired sessions automatically

## [v1.0.50]

### Fixed

- disable demo data seeding by default

## [v1.0.49]

### Added

- localize auth and profile flows

## [v1.0.48]

### Fixed

- place desktop update translations per locale
- localize desktop update banner labels

## [v1.0.47]

### Added

- add interview room status messages

### Fixed

- localize interview room runtime states

## [v1.0.46]

### Fixed

- derive plans from real interview reports

## [v1.0.45]

### Fixed

- hide release metadata assets

## [v1.0.44]

### Fixed

- simplify Dockerfile shell commands
- correct Dockerfile continuation syntax

### Security

- run container as non-root user

## [v1.0.43]

### Security

- remove exposed API key from env example

## [v1.0.42]

### Added

- add interview report translations
- localize interview report and TXT export

### Fixed

- keep frontend package JSON valid
- remove duplicate legacy report download

## [v1.0.41]

### Added

- add frontend/src/i18n/index.js
- add backend/tests/test_i18n.py
- add backend/core/locale.py
- update frontend/src/main.js
- update frontend/src/components/resume/widgets/JobRecommend.vue
- update frontend/src/components/resume/widgets/AIAnalysis.vue
- update frontend/src/components/resume/ResumeUpload.vue
- update frontend/src/components/interview/api.js
- update frontend/src/components/interview/InterviewRoom.vue
- update frontend/src/components/interview/Interview.vue
- update frontend/src/components/home/Home.vue
- update frontend/src/App.vue
- update frontend/pnpm-lock.yaml
- update frontend/package.json
- update backend/services/session_service.py
- update backend/services/ai_service.py
- update backend/schemas.py
- update backend/routers/resume.py
- update backend/routers/interview.py
- update backend/core/database.py

## [v1.0.40]

### Fixed

- remove leaking container healthcheck

## [v1.0.39]

### Fixed

- keep health checks responsive during AI calls

## [v1.0.38]

### Added

- add historical score trend chart on profile page

### Fixed

- scope study records and plans to current user
- do not persist password in localStorage remember-me

## [v1.0.37]

### Fixed

- only show migration notice on old domain

## [v1.0.36]

### Added

- add one-time domain migration notice modal on homepage

## [v1.0.35]

### Fixed

- restore profile avatar fallback

## [v1.0.34]

### Fixed

- remove nested page scrollbar

## [v1.0.33]

### Fixed

- keep generated changelog notes idempotent

## [v1.0.32]

### Fixed

- standardize public release notes sync

## [v1.0.31]

### Fixed

- clean up interview tag merge artifacts
- preserve user-scoped session logic when adding tags

## [v1.0.30]

### Fixed

- refresh my page cache data
- cache my page profile data

## [v1.0.29]

_No user-visible changes in this release._

## [v1.0.28]

### Fixed

- standardize public release notes
- fetch all release notes for changelog
- paginate release notes in changelog
- generate changelog from release notes

## [v1.0.27]

_No user-visible changes in this release._

## [v1.0.26]

### Added

- isolate interview data by authenticated user

## [v1.0.25]

_No user-visible changes in this release._

## [v1.0.24]

### Fixed

- remove unused default job recommendations

## [v1.0.23]

_No user-visible changes in this release._

## [v1.0.22]

_No user-visible changes in this release._

## [v1.0.21]

_No user-visible changes in this release._

## [v1.0.20]

_No user-visible changes in this release._

## [v1.0.19]

_No user-visible changes in this release._

## [v1.0.18]

_No user-visible changes in this release._

## [v1.0.17]

_No user-visible changes in this release._

## [v1.0.16]

_No user-visible changes in this release._

## [v1.0.15]

### Fixed

- simplify resume drag upload handling

## [v1.0.14]

### Added

- add skill package download card

## [v1.0.13]

_No user-visible changes in this release._

## [v1.0.12]

### Fixed

- vercel api endpoint

## [v1.0.11]

### Added

- add docker compose workflow

## [v1.0.10]

### Added

- support Linux desktop update flow
- add desktop auto update flow

### Changed

- simplify desktop update UI

## [v1.0.9]

_No user-visible changes in this release._

## [v1.0.8]

### Added

- render release notes as markdown

### Fixed

- ignore wc total line in APK size check
- compare Android release APKs by hash and size
- always request release metadata via api path
- build real split android release apks
- publish release artifacts without repo sync
- sign android apk outputs in release workflow
- escape newline in apk workflow output
- handle nested android apk outputs
- verify only signed android apks
- use correct android keystore path
- resolve apksigner from android sdk
- stop re-adding android platform in release workflow
- track android project files for release builds
- repair desktop release workflow yaml

## [v1.0.6]

_No user-visible changes in this release._

## [v1.0.5]

### Added

- sign and split Android release APKs
- 下载页样式统一
- add web app download entry

### Changed

- sync public docs and artifacts to release repo

### Fixed

- normalize Android release APK naming
- submit auth form with Enter key

## [v1.0.4]

### Changed

- sync public docs and artifacts to release repo

### Fixed

- publish public artifacts as release assets
- validate release repo token before checkout
- checkout source repo before public sync
- add author email for Linux packaging
- use png icon for Linux desktop builds

## [v1.0.3]

### Added

- 更新示例环境变量以使用新的 AI API 和模型配置
- remenber-password
- 更新构建配置以支持 Linux 和 Windows 的新打包格式

### Changed

- AI Interview frontend with Vue 3, Vite, Electron and Capacitor

### Fixed

- submit auth form with Enter key
- change-delete-style--fix-rename-function
- ts2js
- add capacitor setup for CI sync

## [v1.0.2]

### Fixed

- node 22
- disable implicit electron-builder publishing in ci

## [v1.0.1]

### Added

- 更新 Docker 构建工作流以支持多个分支推送
- 初步统一样式，美化
- gpt换ds
- 图标
- 优化docker部署的磁盘占用问题
- add Electron packaging support for desktop app
- Docker OK
- AI report
- boys with boys' picture/Cheryl
- picture
- I write it in the name of branch/Cherylxb
- merge mock interview room UI into real interview flow and remove mock page
- 完善简历上传功能+fix:修改数据库json变文字 (#14)
- 接入真实数据库数据，保留原有样式，修复前端请求端口和代理问题
- 添加 Vercel 配置文件
- 设计学习计划页面 (#9)
- 设计学习计划页面 (#8)
- 我的页面 - 新增Profile组件和My组件 (#6)
- 在导航栏加入“我的”页面，新增了AI分析页面

### Changed

- 回退style的变更
- 为路由添加名称标识
- 更新构建命令和输出目录
- 整理组件
- reorganize component folders by feature
- 移动并优化 preview 属性的定义位置
- 优化代码格式和结构
- initial project scaffold (Vue + Python 前后端分离架构)

### Fixed

- 美化
- show real username below avatar
- 补路由
- 排查剩下的/api
- 读取.env
- no mock
- fix backend startup path and update docs
- repair plan and detail persistence
- pass round state into new sessions
- isolate home CTA loading states
- 面试官失忆问题
- 修正API代理目标地址
- restore deleted comments and error message
- My页面报错
- 删除多余数据库
- 修复重实例+对接数据库接口

### Removed

- 还原导航栏悬停样式
- 取消 vite 配置的修改

## 说明

- 完整安装包与下载方式见发布仓库：[SsuJojo/AI-Interview-Release](https://github.com/SsuJojo/AI-Interview-Release).

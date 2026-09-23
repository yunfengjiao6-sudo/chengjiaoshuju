# 成交数据看板 · 无数据发布版

本仓库发布 FLIN 楼盘成交数据库的界面、功能源码及 Skill。发布基线为 2026-09-23。

## 下载

完整源码与 Skill 压缩包放在独立分支 [release/data-free-20260923](https://github.com/yunfengjiao6-sudo/chengjiaoshuju/tree/release/data-free-20260923)。下载该分支的 `property-deal-dashboard-20260923-data-free.zip` 并解压，按包内 README 安装。

压缩包包含53个文件；没有真实成交、小区档案、数据库、备份、缓存、导出、测试数据库、截图、录音或私密配置。首次启动为空数据库。仅保留明确虚构的输入格式占位符与内存自检。

## 使用

1. 安装 Node.js 24.14 或更高的24.x版本。
2. 进入解压后的 `property-deal-dashboard` 文件夹。
3. 执行 `npm ci`、`npm test`、`npm start`。
4. 打开 `http://127.0.0.1:3210`。Windows也可按包内说明双击启动。

保留小区档案、成交录入、统计、查重、编辑、导入导出、审计、回收站、备份恢复、截图及离线语音功能。截图识别需要Windows中文OCR语言包；离线语音模型与运行程序需另行安装，见包内说明，不包含原电脑的本地运行时。

发布前89项自动测试通过，全新依赖安装和随包自检通过。每个源码文件的SHA256位于包内 `release-files.json`，压缩包校验值在同分支 `SHA256SUMS.txt`。

不要上传使用后生成的 data、backups、logs、导出、录音、截图、环境私密配置或整个运行目录。

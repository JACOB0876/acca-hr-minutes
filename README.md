# ACCA HR Minutes Skill

用于整理 ACCA Club HR 部门会议纪要和随信通知的可复用 Skill。

默认部门为 **HR**，整理人和通知署名为 **李嘉辰**，姓名缩写为 **LJC**，例会通知群为 **HR耍起俱乐部**。这些默认值可以在具体任务中明确覆盖。

## 下载与安装

- [下载完整 Skill 安装包](dist/acca-hr-minutes.zip?raw=true)
- [查看 Skill 入口](acca-hr-minutes/SKILL.md)
- [安装及跨 Agent 使用说明](acca-hr-minutes/INSTALL.md)

解压后，将整个 `acca-hr-minutes` 文件夹放入目标 Agent 支持的 skills 目录，或使用其本地 Skill 导入功能。必须保留 `assets/` 和 `references/`，不能只复制 `SKILL.md`。

不支持 `SKILL.md` 的 Agent 可以将入口和参考规则作为任务指令加载，并同时提供模板。录音转写、Word 编辑和 PDF 渲染能力由目标 Agent 提供，本包不自带这些运行时能力。

## 包含的内容

```text
acca-hr-minutes/
├── SKILL.md
├── INSTALL.md
├── references/
│   ├── content-and-notice.md
│   └── document-standard.md
└── assets/
    ├── meeting-record-template.docx
    ├── document-standard.pdf
    └── template-preview.png
```

规则涵盖录音、PPT及笔记整理，会议事实与讨论状态区分，出勤、分工、期限处理，通知文案，字体、编号、页码与文件命名，以及 Word/PDF 同步修订和排版验收。

## 使用示例

```text
请使用 acca-hr-minutes 整理本次 HR 例会。
会议日期：实际日期；开始时间：实际时间；地点：实际地点。
出勤：实际出席和请假情况。
附件：本次录音、PPT 或会议笔记。
请同时整理会议纪要、随信通知、Word 编辑稿和 PDF 分发稿。
```

新 Agent 仍需取得本次会议的实际材料。会议日期、次数、地点和出勤不会从历史示例自动继承。

## 验证与范围

已完成 Skill 结构检查、相对资源链接检查、模板原件字节一致性校验、ZIP 完整性检查，以及一次独立 Agent 的只读行为复测。未声称已在所有 Agent 平台完成安装或端到端导出验证。

仓库不包含历史会议录音、转写文本、账号密码、语音模型或 API 凭据。规则按用户确认的会话约定提炼；随包社团模板及文书标准为用户提供的原始文件，未对其第三方再分发权或开源许可作额外声明。

# PhD Legacy Vault

这个仓库用于系统整理博士期间的科研工作、论文发表、生活见闻、思考沉淀、反馈复盘与传承资料。它可以同时作为：

1. **GitHub 仓库**：保存结构化、可版本管理的 Markdown 资料。
2. **Obsidian 知识库**：用双链、标签、MOC 页面连接长期知识。
3. **毕业交接档案**：给未来的自己、师弟师妹、合作者留下可复用资料。

## 使用原则

- **先收集，后整理**：任何未分类内容先放入 `00_Inbox_收集箱/`。
- **一事一页**：一个项目、一篇论文、一次实验、一次会议、一个经验教训，尽量单独成页。
- **显式标注可见性**：每篇笔记建议使用 `visibility: public/internal/private`。
- **敏感内容默认不公开**：未发表结果、审稿意见、合作者隐私、原始数据、经费/合同/个人信息不要提交到公开仓库。
- **用链接替代堆文件**：大文件、数据集、原始 PDF、照片建议放在云盘或本地，只在笔记中记录链接、路径和说明。

## 推荐元数据

每篇 Markdown 可用如下 YAML frontmatter：

```yaml
title: 
created: 2026-05-08
updated: 2026-05-08
type: note # project | paper | meeting | experiment | reflection | lesson | legacy
status: seed # seed | growing | stable | archived
visibility: private # public | internal | private
tags: []
related: []
```

## 增量整理流程

1. **随手收集**：想法、文件、截图、会议纪要先进入 `00_Inbox_收集箱/`。
2. **每周归档**：把 Inbox 内容移动到对应目录，并补齐元数据。
3. **每月复盘**：更新 `01_Dashboard_总览/PhD_Timeline.md`、项目状态和论文状态。
4. **每个项目收尾**：补齐项目页、实验记录、失败经验、代码/数据说明。
5. **每篇论文收尾**：补齐手稿、投稿记录、审稿反馈、rebuttal、发表版本与复盘。
6. **毕业前清理**：统一脱敏、确认公开范围、整理传承资料。

## 目录说明

- `00_Inbox_收集箱/`：临时收集区，避免一开始就分类焦虑。
- `01_Dashboard_总览/`：总入口、时间线、研究地图、发表地图、毕业清单。
- `02_Research_科研工作/`：研究问题、项目、实验、代码、数据、方法、失败记录、会议。
- `03_Papers_论文与发表/`：论文手稿、投稿、审稿、rebuttal、已发表版本、文献笔记。
- `04_Thesis_毕业论文/`：毕业论文大纲、章节、图表、答辩和学校要求。
- `05_Life_生活与见闻/`：博士期间的生活、城市、人物、会议、健康与习惯。
- `06_Thinking_思考沉淀/`：长期思考、科研观、效率系统、职业选择、概念摘录。
- `07_Feedback_反馈与复盘/`：导师、同伴、审稿人、自我复盘和经验教训。
- `08_Legacy_传承资料/`：给师弟师妹的上手指南、清单、FAQ、工具流程。
- `09_Admin_Career_事务与去向/`：CV、申请材料、报告海报、荣誉记录、人脉网络。
- `10_Assets_附件/`：图片、幻灯片、PDF、照片等附件。
- `90_Templates_模板/`：项目、论文、会议、实验、反馈、经验、传承模板。
- `99_Archive_归档/`：不再维护但需要保留的资料。

## 建议的 GitHub 提交节奏

- 小步提交：一次提交只整理一个项目、一次会议或一篇论文。
- 提交信息示例：
  - `add project note for xxx`
  - `update thesis outline`
  - `archive paper rebuttal notes`
  - `add lab onboarding checklist`

## 公开前检查

- 是否包含个人身份证件、电话、地址、邮箱、学号等信息？
- 是否包含未授权的论文 PDF、审稿意见、合作者数据？
- 是否包含未发表的关键实验结果或可被抢发的 idea？
- 是否包含导师、同门、被试、访谈对象的敏感评价？
- 是否需要将仓库设为 private，或只公开脱敏版？


## 11_Skills_个人智能体

`11_Skills_个人智能体/` 用于把这个博士知识库转化为可被 AI 复用的个人 Skill。主 Skill 为 `phd-self-os/`，负责规定 AI 如何检索知识库、如何保持事实边界、如何模仿用户口吻、如何生成传承资料。

建议先维护 `phd-self-os/config/voice_profile.md` 和 `phd-self-os/config/vault_map.md`。当知识库逐渐丰满后，可以用 `evals/test_cases.md` 测试这个 Skill 是否能稳定回答“我做过什么、我怎么看、我会怎样传承”。

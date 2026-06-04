# 贡献指南 · Contributing to Self-Promotion Master

我们欢迎并感谢所有形式的贡献！🎉

无论是提交 bug、新增场景、补充案例、改进文案，还是翻译，我们都欢迎你来参与。

## 📋 目录

- [行为准则](#行为准则)
- [我能贡献什么？](#我能贡献什么)
- [如何开始？](#如何开始)
- [提交流程](#提交流程)
- [风格指南](#风格指南)
- [国际化](#国际化)

---

## 行为准则

请阅读并遵守我们的 [行为准则](CODE_OF_CONDUCT.md)。我们致力于打造一个**包容、尊重、专业**的社区。

---

## 我能贡献什么？

### 🐛 报告问题
- 你试用了某段模板，发现效果不理想
- 你发现某段话"翻车"了
- 你发现有事实性错误

### 💡 提出新内容
- **新场景**：竞聘、答辩、相亲……任何职场相关场景
- **新场合**：互联网大厂、金融/咨询、政府/事业单位
- **新武器**：补充方法论
- **新案例**：你身边真实的 before/after 故事（脱敏后）
- **新强度档**：例如"内敛版"、"奢华版"

### 📝 改进现有内容
- 修正错别字、语病
- 优化表达
- 补充示例
- 翻译成其他语言

### 🔧 工具化
- 写脚本自动生成文本
- 集成到其他工具（Notion 模板、Obsidian 插件等）
- 写 Web 应用

---

## 如何开始？

1. **先读一遍** [`SKILL.md`](SKILL.md) 和 [`README.md`](README.md)，了解项目
2. **在 Issue 里搜索**，看看你的想法是否已被讨论
3. **新建 Issue** 描述你的想法，等 maintainer 确认
4. **Fork + 改 + 提 PR**

---

## 提交流程

### 1. Fork & Clone
```bash
# Fork 后 clone 你的 fork
git clone https://github.com/YOUR_USERNAME/self-promotion-master.git
cd self-promotion-master

# 添加 upstream
git remote add upstream https://github.com/ORIGINAL_OWNER/self-promotion-master.git
```

### 2. 创建分支
```bash
git checkout -b feature/your-feature-name
# 或者 fix/your-bug-name
# 或者 docs/your-doc-improvement
```

### 3. 提交 Commit
我们遵循 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/) 规范：

```bash
git commit -m "feat: 增加互联网大厂晋升答辩调性"
git commit -m "fix: 修复私企案例中的数据不一致"
git commit -m "docs: 改进 README 中的示例"
```

常用前缀：
- `feat`: 新功能
- `fix`: 修 bug
- `docs`: 仅文档
- `style`: 格式（不影响代码运行）
- `refactor`: 重构
- `test`: 添加测试
- `chore`: 构建/工具链

### 4. 推送 & 提 PR
```bash
git push origin feature/your-feature-name
```

然后在 GitHub 上 **Open Pull Request**，填写 PR 模板。

### 5. 等待 Review
- Maintainer 会在 7 天内 review
- 可能有讨论和修改建议
- 通过后会被 merge

---

## 风格指南

### 文案风格
- **简洁**：能用 1 句话不用 2 句
- **有冲击力**：动词要硬、数字要狠
- **有温度**：不要冷冰冰的指令，要有"前辈带后辈"的感觉
- **中英兼容**：核心概念给中英双语版本

### Markdown 规范
- 标题层级不超过 4 层
- 代码块标注语言（```markdown、```bash）
- 表格要有表头
- 链接用相对路径（`./SKILL.md` 而非绝对 URL）
- 重要内容用 `>` 引用块

### 案例格式
所有 before/after 案例请遵循以下结构：

```markdown
## 案例 X：[场景] · [场合]

### 原始版（你写的）
> [原文]

### 标准版
> [润色后文本]

### 激进版（可选）
> [再润色后的文本]

### 关键改动说明

| 原文 | 润色后 | 用了什么武器 |
|---|---|---|
| ... | ... | ... |
```

### 命名规范
- 文件名：全小写、用连字符（`tones-private.md` 而非 `TonesPrivate.md`）
- 场合调性文件：`tones-{场合}.md`
- 场景模板文件：`scenario-{场景}.md`
- 案例文件：`example-{类型}-{场合}.md`

---

## 国际化

我们目前主推中文版本，欢迎翻译到其他语言。

### 添加新语言的步骤
1. 在 `README.md` 顶部添加你的语言链接
2. 翻译 `README.md` 和 `SKILL.md`（先翻译这两个最关键）
3. 在 `references/` 下添加 `i18n/` 目录（如 `references/i18n/en/`）
4. 在 PR 中说明翻译覆盖范围

### 已支持 / 进行中的翻译
- [x] 中文（zh-CN，原版）
- [ ] English（计划中，欢迎 PR）

---

## ❓ 我有问题想问

- 在 [Discussions](https://github.com/your-username/self-promotion-master/discussions) 开帖
- 简单的 bug/feature 直接开 issue

---

## 🙏 致谢

所有贡献者都会在 [README.md - 致谢](README.md#致谢) 中列出。

再次感谢你的贡献！❤️

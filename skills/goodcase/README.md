# goodcase Skill

## 安装 / Install

```bash
# Claude Code（复制到用户级 skills 目录）
cp -r skills/goodcase ~/.claude/skills/goodcase
```

其他兼容 SKILL.md 的平台（Codex CLI / Cursor / Gemini CLI 等）：把 `skills/goodcase/` 目录复制到对应平台的 skills 目录即可。

## 是什么 / What

让 AI Agent 直接查询 [goodcase.ai](https://goodcase.ai) 上人工精选的 AI 爆款案例：真实出处、创作者署名、完整 Prompt、推荐模型、稳定分与成本档。公开 API，无需任何 Key。

Lets AI agents query hand-curated viral AI cases from [goodcase.ai](https://goodcase.ai): real sources, creator attribution, full prompts, recommended models, stability scores and cost bands. Public API, no key required.

接口连不上或被限流时，Skill 会改查随包附带的离线数据（`references/`，各分类稳定分最高的一批案例），并在回答里标明数据日期。

When the API is unreachable or rate-limited, the skill falls back to the bundled offline snapshot in `references/` (the top cases by stability score in each category) and states the snapshot date in its answer.

## 用法 / Usage

装好后直接问 Agent，例如：

- 「找几个 AI 视频的爆款案例」
- 「有没有玻璃质感的图像 prompt」
- 「这条 case 的完整提示词给我」
- 「给我的公众号文章配张图」，选定一条后再说「用第 2 条，换成我的主题」

Just ask your agent things like "show me viral AI video cases" or "find a prompt for glass-texture images" — the skill routes to the goodcase.ai public API automatically.

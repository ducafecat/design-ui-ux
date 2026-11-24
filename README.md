# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.en.md) | 简体中文

为需要移动端或 PC 端界面设计的开发者和产品团队提供一套可执行的 **UI/UX 设计 Agent Skill**：从真实模板参考、逐题风格访谈，到自包含 HTML + Tailwind 设计稿与浏览器验收。

默认交付 `design/index.html`，将业务视图、交互、素材和样式标准内置到一个文件中。项目处于初始整理阶段；尚未发布远程仓库，也不宣称已上架技能目录或通过跨客户端验证。

## 工作流程

1. 明确业务、目标端和页面范围。
2. 考察至少 5 个模板来源，每轮展示 6 张真实截图，交付 `design/preview.html`。
3. 选中参考后逐题访谈，确认风格方案。
4. 制作单文件 HTML，内嵌编译后的 Tailwind CSS、脚本、素材及样式标准。
5. 在独立目录中以 `file://` 验证，记录实际检查与限制。

局部修改沿用现有规范；用户可以明确跳过参考选择或访谈阶段。

## 安装到项目

本仓库包含一个技能：[design-ui-ux](skills/design-ui-ux/SKILL.md)。在已取得仓库副本的目录运行：

```bash
mkdir -p /absolute/path/to/your-project/.agents/skills
cp -R skills/design-ui-ux /absolute/path/to/your-project/.agents/skills/
```

将 `/absolute/path/to/your-project` 替换为目标项目路径；若目标目录已存在该技能，先备份并比较后更新。让支持 Agent Skills 的客户端读取 `.agents/skills/design-ui-ux/SKILL.md`；具体自动发现规则由客户端决定。本仓库提供目录结构，未保证所有客户端即装即用。

### 环境要求

- 本地数据检索使用 Python 3，仅依赖标准库；无 Python 时可沿用详细规范，但不能声称完成检索。
- 完整设计流程需要浏览器、真实截图和本地 HTML 预览能力；默认优先 Ego Lite，需另行配置 `ego-browser` 技能。不可用时按技能规则说明并使用替代浏览器。
- 制作阶段需要可编译 Tailwind 的工具；最终成品应不依赖 Node.js、CDN 或运行时构建。

## 使用示例

在已加载此技能的 Agent 中输入：

> 使用 design-ui-ux，为健身课程预约产品设计移动端界面，包含课程列表、详情和预约结果，默认输出到 design/。

预期先得到需求摘要和参考选型页；选定参考并确认风格后得到 `design/index.html`，其中有样式标准入口。此仓库提供技能与检索数据，不包含预先制作的健身 App 或真实预约后端。

局部修改示例：

> 使用 design-ui-ux，检查现有 design/index.html 的表单间距和键盘焦点，沿用现有视觉风格修复。

## 本地检索与检查

从仓库根目录执行：

```bash
python3 skills/design-ui-ux/scripts/search.py "keyboard focus modal" --domain ux
python3 skills/design-ui-ux/scripts/search.py "responsive form navigation" --stack html-tailwind
python3 skills/design-ui-ux/scripts/validate_data.py
```

前两条返回候选设计建议；最后一条检查数据完整性。它们不会验证实际生成页面的视觉或交互质量。详细规则见[检索指南](skills/design-ui-ux/references/search-guide.md)。

## 目录与文档

| 路径 | 内容 |
| --- | --- |
| [SKILL.md](skills/design-ui-ux/SKILL.md) | 激活条件、工作流程与交付要求 |
| [设计规范](skills/design-ui-ux/references/design-standards.md) | 视觉、交互、无障碍与目标端规范 |
| [访谈问题库](skills/design-ui-ux/references/style-interview.md) | 参考选定后的逐题访谈 |
| `skills/design-ui-ux/scripts/` | Python 检索与数据检查 |
| `skills/design-ui-ux/data/` | 风格、颜色、字体及交互参考数据 |
| [GitHub 发布配置](docs/github-metadata.md) | About、Topics 与发布检查 |

## 反馈、维护与许可

提交改进前阅读 [CONTRIBUTING.md](CONTRIBUTING.md)，版本记录见 [CHANGELOG.md](CHANGELOG.md)，敏感问题见 [SECURITY.md](SECURITY.md)。远程仓库建立后使用其 Issues 反馈可复现问题。

当前未指定项目许可证，不能据此认定为已授权的开源项目。发布前需由维护者确认代码与数据的来源、再分发权及许可证；数据中的来源记录不等于再分发授权。参见 [来源说明](NOTICE.md)。

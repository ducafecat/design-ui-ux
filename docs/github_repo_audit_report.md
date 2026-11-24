# GitHub 仓库审计报告

## 1. 执行摘要

审计日期：2026-11-24（Asia/Shanghai）。目标为本地 `ducafe-skills-design-ui-ux`，定位是面向开发者与产品团队的 UI/UX Agent Skill，以真实参考、风格访谈和单文件 HTML + Tailwind 原型为核心交付。

**诊断得分 65/100，证据覆盖率 78%。** 这是本地发布准备度与文档的诊断，不能解释为公开 GitHub SEO 得分、官方评分或排名预测。远程身份未确定，About、Topics、流量及公开收录均未知。

前三项行动：① 发布前确认代码和数据再分发授权及项目许可证；② 在干净项目验证安装、发现与完整原型交付，形成真实演示；③ 确定公开仓库身份后应用元数据并建立公开基线。当前没有已确认 P0。

本次仅更新本报告，未提交、推送、修改设置或执行项目代码。报告包含尚未证实已公开的本地项目状态；对外发布前由维护者审核。未包含凭据或私密流量数据。[E001–E007]

## 2. 范围和证据快照

| 项目 | 当前值 | 证据 |
|---|---|---|
| 本地名称 | ducafe-skills-design-ui-ux | E001/E003 |
| Repository URL / visibility / default branch | UNKNOWN；`git remote -v` 无输出，不能据此断言 GitHub 上不存在仓库 | E001 |
| 本地分支 / HEAD | main / 68ae358f89a3912d7def9a9c1bcc325e90757f83 | E001 |
| 工作区 | 审计前干净；本次只改报告 | E001/E010 |
| 最近本地提交 | 2026-11-24T23:40:13+08:00；不等于远程 push 时间 | E001 |
| Stars / forks / subscribers / issues与PR / 最近push | UNKNOWN，无已确认远程对象 | E002 |
| 类型 / 受众 / 转化 | 单技能仓库；开发者和产品团队；复制安装后成功完成原型 | E003/E004 |
| 工具 / 时间 | Git、技能离线辅助脚本、文件静态检查、公共网页检索；2026-11-24 15:40–15:50 UTC | E001–E010 |

未调用目标 GitHub API、traffic、注册表接口；无权限错误可报告。未安装依赖、运行仓库检查或客户端设计流程。只运行审计工具及只读路径检查。外部研究仅使用通用公开词与公开项目，未将本地代码提交外部服务。

## 3. 评分与检查结果

PASS=全权重，PARTIAL=半权重，FAIL=0；UNKNOWN 从已知权重排除，非失败。没有 NA。

| ID | 维度 | 权重 | 状态 | 证据 / 理由 | 得分 |
|---|---|---:|---|---|---:|
| D01 | 命名 | 6 | PASS | E001/E003；本地名称清晰，建议保留，迁移风险见第4节 | 6 |
| D02 | About | 6 | UNKNOWN | E002；远程未确认 | — |
| D03 | Topics | 5 | UNKNOWN | E002；建议文件不等于已配置 | — |
| D04 | Website | 3 | UNKNOWN | E002；官方主页字段未知 | — |
| D05 | 关键词与搜索 | 6 | PARTIAL | E008/E009；有同类公开样本，目标Topics和搜索表现未知 | 3 |
| R01 | README可读 | 5 | PASS | E003；本地双语文档可读 | 5 |
| R02 | 价值主张 | 4 | PASS | E003；受众、流程、输出和限制明确 | 4 |
| R03 | 安装 | 5 | PARTIAL | E003/E004；复制路径吻合，客户端发现未试验 | 2.5 |
| R04 | 使用 | 5 | PARTIAL | E003/E004；具体提示词和预期产物，无端到端记录 | 2.5 |
| R05 | 链接 | 4 | PASS | E007；README 21条及技能8条相对链接目标存在，无外链/锚点待核验 | 4 |
| R06 | 结构与演示 | 4 | PARTIAL | E003；导航清晰，有文字示例但缺实际成品演示 | 2 |
| R07 | 本地化 | 2 | PASS | E003；双向导航、安装、命令、限制与许可一致，英文明确主体中文 | 2 |
| T01 | 许可证 | 5 | FAIL | E005；无项目许可，NOTICE明确授权未确认 | 0 |
| T02 | 贡献与反馈 | 4 | PARTIAL | E005；指南和模板具体，实际反馈入口未配置 | 2 |
| T03 | 安全政策 | 3 | PARTIAL | E005；隐私指导明确，可用私密联系渠道未配置 | 1.5 |
| T04 | 维护透明度 | 3 | PASS | E003/E005；初始化状态、兼容性和响应限制明确 | 3 |
| E01 | 发布策略 | 4 | PARTIAL | E005；0.1.0与变更记录一致，升级策略不足，远程release未知 | 2 |
| E02 | CI与测试 | 4 | PARTIAL | E006；检查命令有意义，但运行结果未核验 | 2 |
| E03 | 专项分发 | 4 | PARTIAL | E004；技能结构和引用有效，实际客户端分发未验 | 2 |
| E04 | 发布安全 | 3 | UNKNOWN | E002；仅文件清单不构成安全检查完成 | — |
| G01 | 外部发现 | 5 | UNKNOWN | E002/E008；无目标公开身份，不能核验其索引与目录 | — |
| G02 | 同类差异化 | 5 | PASS | E009；三个同类项目的直接公开证据 | 5 |
| G03 | 衡量 | 5 | PARTIAL | E001/E007；本地基线与复查方法已建立，无公开数据 | 2.5 |

| 分组 | 适用权重 | 已知权重 | 获得分 | 覆盖率 |
|---|---:|---:|---:|---:|
| Discovery | 26 | 12 | 9 | 46% |
| README | 29 | 29 | 22 | 100% |
| Trust | 15 | 15 | 6.5 | 100% |
| Engineering | 15 | 12 | 6 | 80% |
| Growth | 15 | 10 | 7.5 | 67% |
| 合计 | 100 | 78 | 51 | 78% |

Score = round(100 × 51 / 78) = 65；Coverage = round(100 × 78 / 100) = 78%。整体覆盖超过70%，但公开发现子项证据不足，不能与全线上审计直接比较。

## 4. GitHub SEO 与仓库元数据

保留 `ducafe-skills-design-ui-ux`。`ducafe` 可作为品牌前缀，后半段对应技能类别。尚无证据说明改名有收益；未来改名会影响 clone、技能安装地址、文档及外部链接，重定向也不能替代逐项验证。[E001/E003]

当前 About、Website、Topics、社交预览：均 UNKNOWN。`docs/github-metadata.md` 仅为建议。[E005]

建议英文 About（未应用）：

> UI/UX design skill for developers and product teams: real template references, style interviews, and self-contained HTML + Tailwind prototypes.

中文对应：面向开发者与产品团队的 UI/UX 设计技能，通过真实模板参考与风格访谈，交付自包含 HTML + Tailwind 原型。

Topics：现有/保留/移除均无法判断；建议新增候选按优先级为 `agent-skills`, `ui-design`, `ux-design`, `html-prototype`, `tailwindcss`, `prototyping`, `design-workflow`, `responsive-design`, `design-system`，共9个，均为合法语法。仅在实际能力保持一致时采用，不添加未验证的客户端兼容标签。

Website 仅填写真实、可访问、维护者控制的示例或文档页；没有则暂不填。社交预览建议使用项目名、“Reference → Interview → Prototype”及一张获授权真实成品截图，保证缩略图可读。未观察图片，不宣称已有自定义预览；上传尺寸需发布时查官方要求。

## 5. README、文档与安装转化

现有首屏明确输出 `design/index.html`；工作流程、复制安装、环境、两类使用示例、搜索命令及许可限制齐全。新用户需取得副本、复制技能、让客户端加载、提出任务、选参考与风格，再验收成品；取得副本尚无公开入口，完整路径未验证。未见虚构徽章或安装量。[E003]

本地链接检查：中文11条、英文10条、技能8条均存在；该结果只证明路径可达，不证明 GitHub 渲染或浏览器体验。没有目标 README 外链和锚点需要 HTTP 检查。[E007]

建议 H1（可保持现有英文定位）：

```text
Design UI UX — Agent Skill for Self-Contained HTML + Tailwind Prototypes
```

建议英文首段：

> Design mobile and desktop UI prototypes through real template references, focused style interviews, and browser validation. Built for developers and product teams, this Agent Skill delivers a single HTML file with compiled Tailwind CSS and an embedded style guide.

这是能力定位，不能写成已经完成跨客户端验收的保证。建议结构：价值与成品预览 → 环境与安装 → 首次任务及预期产物 → 两种使用路径 → 检索 → 兼容性与排障 → 维护与许可。优先补充一份真实授权示例，再扩充文案。

建议 Quick Start（路径经静态核对；本次未执行安装）：

```bash
# 在本仓库根目录，将目标替换为实际项目绝对路径；已有技能先备份比较。
mkdir -p /absolute/path/to/your-project/.agents/skills
cp -R skills/design-ui-ux /absolute/path/to/your-project/.agents/skills/
```

随后在支持相应目录的客户端加载技能，输入 README 健身预约示例。验收应看到参考页、确认记录以及可独立打开的 `design/index.html`，且包含可返回的样式标准入口。支持的 Python 最低版本和 Tailwind 作者工具版本未定义；CI仅声明 Python 3.11，不等于支持全部 Python 3。建议补充技能未发现、浏览器不可用、Tailwind无法编译三种排障，以及更新/卸载时只处理对应技能目录的说明。双语 README 同步检查命令、依赖、输出及限制。

## 6. 社区、信任与工程健康

`NOTICE.md` 明确技能从本机已有目录复制，追溯文件不等于授权；无 LICENSE，不能宣称具备开源许可。建议逐类核验脚本、数据、字体和图标来源后决定许可与署名，而非直接套用 MIT；本审计未作法律结论。[E005]

贡献指南要求客户端/Python版本、触发词、预期与实际结果，并禁止敏感资料。Issue/PR模板存在，但无已确认远程入口。安全政策明确不要公开敏感细节，然而私密入口和联系方式没有配置，需发布前补足。未检索目标 issue/PR 样本，也无法判断组织默认社区文件；小型初始项目缺少行为准则不单独视为缺陷。

CI使用 `contents: read`、Python 3.11，执行数据检查及一条UX搜索；另有多份测试源码，但工作流没有运行测试套件。不能用文件存在声称 CI 通过或全部测试已运行。[E006]

## 7. 发布与项目类型专项

| 专项 | 本地观察 | 状态 |
|---|---|---|
| 路径/name | skills/design-ui-ux/SKILL.md；name=design-ui-ux，目录吻合 | PASS |
| description | 中文描述激活条件、输出及局部调整，长度小于1024字符 | PASS |
| 渐进读取 | 主文件68行，细节放references；8条相对链接存在 | PASS |
| 安装 | cp复制整个技能目录，包含scripts/data/references | 静态吻合，运行未验 |
| 依赖 | Python、本地浏览器及Tailwind编译；ego-browser可替代 | 依赖明确，版本矩阵不足 |
| 失败处理 | 浏览器/编译不可用需说明缺口，不伪造检查 | 有明确指导 |
| 兼容性 | README明确没有跨客户端保证 | 实际兼容性UNKNOWN |
| 版本/分发 | private package 0.1.0，本地CHANGELOG；不是npm分发产品 | 远程release/tag/catalog UNKNOWN |

数据清单有12个领域文件及22个stack文件，但不是覆盖质量或原生端实现保证。来源文件含2026-08-12核验、90天needs-review策略；截至11月24已超过90天，属于应调查的数据时效风险，未执行校验，不判定脚本失败。[E004/E006]

## 8. 搜索关键词与竞品

| Keyword | Intent | 观察来源 | 建议位置 | 优先级 |
|---|---|---|---|---|
| UI UX design agent skill | 寻找可加载设计技能 | E008/E009同类公开页面 | About/H1 | 高 |
| HTML prototype | 产出可交互原型 | E009原型技能 | Topics/示例 | 高 |
| self-contained HTML Tailwind prototype | 独立携带与离线演示 | E003/E004本地能力；搜索量未知 | 首屏/长尾文档 | 高 |
| design workflow | 参考选择与设计决策 | E009流程型项目 | Topics/流程 | 中 |

| Query | 日期/来源 | 窗口/sort | 观察 | Incomplete |
|---|---|---|---|---|
| github UI UX design agent skill HTML Tailwind prototype | 2026-11-24 / web搜索 | 工具返回摘要；引擎默认 | 出现HTML原型相关项目 | 工具未提供 |
| github anthropics skills frontend-design | 同上 | 同上 | 出现官方技能路径相关结果 | 工具未提供 |
| github nextlevelbuilder ui ux pro max skill | 同上 | 同上 | 出现项目代码页和目录结果 | 工具未提供 |
| github pbakaus impeccable design skills | 同上 | 同上 | 混合结果，未选作已核验竞品 | 工具未提供 |

以上是公共网页搜索样本；工具未说明Google/Bing后端，不能归为特定引擎。没有GitHub API排序、目标精确名查询或排名；因远程身份未知，没有将未发布目标名称用于公开检索。[E008]

样本以“相同开发者受众、Agent技能、前端设计或HTML原型”为标准，同时纳入小型项目，不按星数选择。以下结论仅基于读取到的页面，不代表运行评测。[E009]

| Competitor | 可比性/定位 | 入门与演示 | 发布/信任/分发 | 本项目机会 |
|---|---|---|---|---|
| [scanadi/design-skill](https://github.com/scanadi/design-skill) | 可携带设计技能；强调既有设计语言 | README提供安装与首次设置流程 | 页面显示MIT与安装脚本；release未查 | 展示单文件搬运、样式标准与隔离打开证据 |
| [SwiftyJunnos/design-ui-prototypes](https://github.com/SwiftyJunnos/design-ui-prototypes) | UI方向、交互原型和交接 | README给出分阶段产物和命令 | Topics含html-prototype；链接skills.sh但未独立核验目录 | 突出真实模板选型与可跳过阶段的局部修改路径 |
| [anthropics/skills frontend-design](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md) | 前端视觉设计指导 | 主体强调有意图的布局与字体 | frontmatter引用LICENSE.txt；非仓库整体许可结论 | 用真实产物证明从选择参考到浏览器验收的流程 |

关键词没有搜索量或难度数据。差异化是流程与交付约束的推断，不能声称质量优于竞品。

## 9. 外部搜索与分发

目标Google/Bing收录、skills.sh上架、npm及社交预览均 UNKNOWN。没有公开URL就无法有效核验目标目录条目；搜索无结果也不构成未被索引的证据。[E002/E008]

建议授权确认后：先发布自有示例及教程，再核验技能目录的实际安装与展示，最后向允许项目分享的相关社区发布真实案例。说明自己是维护者，不批量私信、不购买星标。发布文章链接真实仓库与示例；GitHub页面HTML头、robots和搜索引擎排名不可由仓库作者直接配置。

## 10. 流量与衡量

旧报告日期同为2026-11-24，记录当时无提交、无origin且没有数值评分；本次已出现本地提交，origin仍无，不能将本次评分视为增长幅度。旧报告称数据检查通过，仅作为历史自述，本次没有重新验证。[E000/E001]

| KPI | 基线/窗口 | 来源 | 下一次检查 | 局限 |
|---|---|---|---|---|
| 文档链接缺失 | 当前抽查29条，0缺失 | E007 | 每次文档变更后 | 只覆盖相对路径 |
| 安装/首次交付成功 | UNKNOWN | 无运行记录 | 首次发布前记录客户端和版本 | 不是自动化检查结果 |
| Stars/forks | UNKNOWN | 远程未确认 | 发布日与+30/+90天快照 | 不是安装数 |
| 14天views/clones/unique | UNKNOWN | 未请求私密traffic | 获适当授权后建立同长窗口 | 克隆不等于成功安装，unique不能跨窗口求和 |
| 公开查询样本出现 | 目标UNKNOWN；同类研究见第8节 | E008 | 发布后相同查询及窗口 | 不是完整索引和排名 |
| 目录安装指标 | UNKNOWN | 无已验证listing | 实际上架后记录来源和日期 | 不混同访问、安装和星标 |

先建立基线，再制定数值目标；不承诺自然增长或因果SEO收益。

## 11. 风险、发现与行动计划

以下为唯一优先行动表；所有内容均为建议，未实施。

| ID | 优先级 | 信心 | 证据 | 实际 vs 预期 | 影响 | 修复/位置 | 工作量 | 依赖 | 验收 |
|---|---|---|---|---|---|---|---|---|---|
| F01 | P1 | 高 | E005 | 无项目许可且来源授权未确认；发布需许可范围清楚 | 用户无法确认使用/再分发权限 | 核验来源、补LICENSE和NOTICE | M | 维护者/必要的权利人 | 逐类来源可追溯，许可/署名/文档一致 |
| F02 | P2 | 高 | E003/E004 | 静态安装与提示词有，完整流程无证据 | 首次使用成功率未知 | 干净项目试装并补真实示例与兼容性矩阵 | M | 浏览器、Tailwind、选定客户端；公开示例依赖F01 | 记录发现路径、版本、产物、file打开及交互检查 |
| F03 | P2 | 高 | E001/E005 | origin未配置；公开身份未核验 | 无法验证发现与反馈路径 | 确定真实公开URL，配置第4节元数据并更新文档入口 | S | 发布授权与F01 | API或页面可核验身份、字段、默认分支和安装地址 |
| F04 | P2 | 高 | E005 | 安全指导有，可用私密入口无 | 敏感问题难以私下反馈 | SECURITY.md及实际私密报告入口 | XS | F03或维护者提供真实私密渠道 | 可见且可用，不需要公开敏感细节 |
| F05 | P2 | 高 | E006 | CI只做数据和搜索检查，测试源码未被工作流执行 | 回归状态不透明 | 评估测试范围，增加适用检查并记录状态 | S | 测试运行需后续实施授权 | 默认分支实际运行可查，不把存在等同通过 |
| F06 | P2调查 | 中 | E006 | 来源核验日期超过部分90天策略 | 数据时效可能影响建议 | 复核provenance与时效处理规则 | S | 具体记录来源与后续执行验证 | 明确过期记录处理；不以本报告推断校验失败 |

7天（至2026-12-01）：维护者完成F01决策，验证F02，明确F03身份；首个里程碑是可复现使用证据。30天（至2026-12-24）：维护者/文档负责人完成F04–F06，发布真实演示与首份版本说明，建立相同窗口基线。90天（至2027-02-22）：维护者复核兼容性、相同公开查询样本与渠道效果，保留有效渠道。日期为建议节点，未创建定时任务。

## 12. 建议改稿与验收

可复制About/Topics见第4节；README首屏和Quick Start见第5节。发布公告建议顺序：目标用户 → 一份真实任务 → 参考/确认/成品截图 → 实际安装路径 → 验证过的客户端与版本 → 已知限制 → 许可证与反馈入口。不要使用未经验证的性能、采用量或兼容性宣称。

后续可手动执行的建议命令（本审计未运行）：

```bash
python3 skills/design-ui-ux/scripts/validate_data.py
python3 skills/design-ui-ux/scripts/search.py "keyboard focus modal" --domain ux
python3 skills/design-ui-ux/scripts/search.py "responsive form navigation" --stack html-tailwind
```

F01通过条件是授权证据与许可文本齐备，不是创建任意LICENSE文件。F02需验证真实产物复制到空目录仍能打开、导航与样式入口可用，未接后端操作明确标记；结果如失败需保留限制。F03需区分本地HEAD与公开默认分支，再更新“未发布”等状态说明。F04需实际可用渠道；F05需真实检查结果；F06需来源和时效判断记录。

保持仓库名和技能目录可减少安装迁移。实施阶段逐项审核差异，升级前备份既有技能；如需回退，恢复对应文档或安装副本，不删除无关用户产物。本次预期差异仅本报告，不包含上述改动。

## 13. 证据日志与局限

本地证据范围均为HEAD `68ae358f89a3912d7def9a9c1bcc325e90757f83`对应的初始干净工作区；本报告本身为随后修改。公共页面是可变页面，未取得固定commit，不伪造permalink。

| ID | UTC观察时间 | 范围 | 来源/命令 | 观察及限制 |
|---|---|---|---|---|
| E000 | 2026-11-24 15:40–15:41 | 审计前报告 | docs/github_repo_audit_report.md旧版 | 初始化记录称无提交、无origin；无数值评分；历史运行自述未复验 |
| E001 | 2026-11-24 15:40–15:42 | 本地Git | git remote -v；git status --short；git rev-parse HEAD；git branch --show-current；git log -1 | 无remote，初始干净，main，完整SHA见第2节；不证明线上不存在 |
| E002 | 2026-11-24 15:41 | 离线自动证据 | node /Users/ducafecat/.agents/skills/github-repo-audit/scripts/audit.mjs --offline | 成功写入初稿；启发式57分/34%覆盖已被人工评分替换；未访问目标API |
| E003 | 2026-11-24 15:40–15:42 | 本地文档/manifest | README.md、README.en.md、package.json | 双语安装、任务、限制；private=true，0.1.0；未证实npm发布 |
| E004 | 2026-11-24 15:40–15:43 | 技能 | skills/design-ui-ux/SKILL.md及references/design-standards.md、delivery-checklist.md、search-guide.md | 主体68行，frontmatter匹配，输出与失败行为明确；静态检查不验证生成效果 |
| E005 | 2026-11-24 15:41–15:42 | 社区与发布文档 | CONTRIBUTING.md、SECURITY.md、NOTICE.md、CHANGELOG.md、docs/github-metadata.md；git ls-files | 无LICENSE，授权未确认，无实际远程和私密渠道；模板存在，未读取目标远程社区默认文件 |
| E006 | 2026-11-24 15:41–15:43 | 工程与数据 | .github/workflows/validate.yml；scripts/search.py、core.py、validate_data.py；scripts/tests/清单；data/data-provenance.json | 静态检查命令/标准库导入/测试清单；来源时间样本；未运行目标代码或全量时效扫描 |
| E007 | 2026-11-24 15:43–15:45 | 本地路径检查 | Python标准库提取README.md/README.en.md/SKILL.md的Markdown链接并检查Path.exists | 11/10/8条，缺失均0；有限正则经人工读取确认；不评估浏览器渲染 |
| E008 | 2026-11-24 15:41–15:43 | 公共web搜索 | 第8节四条通用查询 | 发现同类项目；工具未说明引擎/全量窗口/incomplete，不构成Google/Bing收录核验 |
| E009 | 2026-11-24 15:42–15:44 | 公共同类页面 | https://github.com/scanadi/design-skill ； https://github.com/SwiftyJunnos/design-ui-prototypes ； https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md | 直接读取定位、流程及页面许可线索；未运行安装，未验证各自release或目录指标 |
| E010 | 2026-11-24 15:40–15:50 | 报告完整性 | 文件检查、评分复算、git status --short | 完整13节；23项评分；最终仅报告变动；工具输出以最终检查为准 |

局限：无目标远程身份，未读取其About/Topics/Website/Release/Actions/Traffic/Community API；Google/Bing与目标目录未独立核验；没有截图或社交预览视觉检查；没有运行目标检查、跨客户端验证、秘密历史扫描、依赖安全或全面授权审查。名称和文件存在不能替代公开状态或运行质量。本报告只保存必要的本地摘要，公开前需审核尚未发布的信息。

交付路径：`docs/github_repo_audit_report.md`。

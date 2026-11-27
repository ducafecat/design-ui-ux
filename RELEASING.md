# 版本与发布

## 当前状态

项目处于早期维护阶段。`package.json` 的 `0.1.0` 与现有初始化变更记录对应；`private: true` 表示它不是待发布的 npm 包。技能目前通过 GitHub 仓库安装。

尚未建立首个 GitHub tag/Release。来源授权仍待核验，详见 [NOTICE.md](NOTICE.md)。本文件是发布流程，不代表已经发布或通过运行验收。

## 版本规则

采用 `MAJOR.MINOR.PATCH`，tag 使用 `v` 前缀。正式发布时，版本号、package.json、CHANGELOG 与 tag 必须一致。

- PATCH：兼容的文档、翻译、数据或缺陷修正。
- MINOR：新增兼容能力或工作流。
- MAJOR：稳定版的破坏性变更；处于 0.x 时，破坏性变化提升 MINOR 并明确迁移步骤。

不追改已发布 tag。撤回有问题的版本时说明原因，修复后发布新版本。现有 `0.1.0` 是初始化记录，是否作为首个发布版本须在发布时核对提交范围。

## 发布前检查

1. 完成 NOTICE 中来源与授权核验，补齐适用许可证、第三方声明及署名；未完成则不创建正式 Release。
2. 选定待发布提交，确认 Git 工作区状态与 GitHub CI；将实际用户变化从 `Unreleased` 整理到版本条目，填写实际发布日期。
3. 运行数据检查；涉及检索实现或数据契约时运行完整测试。以下命令须由执行者记录实际结果，不以命令存在视为通过：

   ```bash
   python3 skills/design-ui-ux/scripts/validate_data.py
   python3 -m unittest discover -s skills/design-ui-ux/scripts/tests
   ```

4. 检查 8 种语言、英文兼容入口、所有语言导航、images 路径与许可说明一致。
5. 在干净的临时项目安装候选提交对应的技能，记录安装来源、实际提交 SHA、客户端和 Node/Python/编译器版本；候选提交与默认分支一致时可使用以下仓库安装入口，安装后仍需核对所用提交：

   ```bash
   npx skills add ducafecat/design-ui-ux --skill design-ui-ux
   ```

6. 完成一个最小原型：真实参考选择、风格确认、实现和浏览器验收。将最终 HTML 复制到空目录，以 `file://` 打开，检查核心功能不依赖相邻文件、CDN 或运行时构建，内置样式标准可访问。记录截图、视口、操作结果与限制。
7. 保存下列验收事实，并标记未完成项：候选 SHA、安装来源、客户端与系统版本、检查命令及退出结果、最终产物路径、浏览器操作和已知限制。未完成端到端验收时不声明兼容性通过。
8. 维护者核对版本号与提交，提交版本变更后再创建对应 tag/Release；Release 说明包含变化、安装、升级、兼容性、许可和已知限制。此流程不自动提交、打 tag 或发布。

## 最近一次本机验证（2026-11-27）

- 数据检查通过：12 个 domain 文件、22 个 stack 文件与 ui-reasoning.csv。
- 文档相对链接、代码块、所有 README 的本地图路径及英文兼容入口一致性检查通过。
- 完整 unittest discovery 未通过：130 个测试通过，另有 2 个模块导入错误（runner 合计 132 项）。`test_catalog_refresh.py` 找不到 `scripts/refresh-google-fonts.py` 与 `scripts/refresh-icon-catalog.py`；`test_relevance_evaluator.py` 找不到 `scripts/evaluate-relevance.py`，模块寻找上级目录时触发 `StopIteration`。这些工具未包含在当前仓库中。
- 修复方向：确认原始上游及授权后补齐对应工具并适配当前目录；如维护者决定不分发这些工具，需明确调整测试范围及维护说明。不要跳过这两项后宣称完整套件通过。
- 未执行技能安装和最终 HTML 浏览器验收，跨客户端兼容性仍未验证。

授权核验、缺失工具引发的测试错误、端到端验收是当前正式发布的未完成条件。上面的版本和流程说明不能替代这些检查。

## 下一版发布说明草稿

以下为尚未发布的文档变化，实际发布时需核对范围、补充版本与验收结果：

- 英文作为默认 README，提供 8 种语言及统一语言导航。
- 所有 README 图片统一引用仓库 images/。
- 更新私密安全报告入口、贡献和多语言维护约定。
- 修正来源说明路径并列明尚待核验的授权范围。
- 增加版本、升级与发布验收流程。

安装和使用步骤见 [README.md](README.md)。代码/数据行为与客户端兼容性须按实际验收结果说明，不由文档修订推断。

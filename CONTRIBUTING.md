# 贡献指南

项目处于早期维护阶段。请通过 [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues) 描述需求或问题，附触发提示词、客户端与 Python 版本、提交 SHA、预期结果和实际结果；移除私密业务信息和凭据。敏感问题请按 [SECURITY.md](SECURITY.md) 使用私密报告入口。维护者目前不承诺固定响应时限。

## 技能与数据变更

- 保持技能目录名与 `SKILL.md` frontmatter 的 `name` 一致，确保引用文件存在。
- 新增或替换数据时，记录上游 URL、版本或提交、采集日期、修改内容、适用许可及再分发依据，并保留必要署名。不要复制授权不明的模板、代码、字体或图片。
- 运行 `python3 skills/design-ui-ux/scripts/validate_data.py` 并记录结果。修改检索逻辑或数据契约时，再运行 `python3 -m unittest discover -s skills/design-ui-ux/scripts/tests`。
- 涉及设计流程时，附实际交付证据；数据校验不能替代浏览器验收。注明客户端、依赖版本、视口、关键操作与未完成检查。

## 多语言文档

默认入口为英文 `README.md`，`README.en.md` 保留为兼容入口，两者内容必须一致。其余语言为简体中文、繁体中文、日语、韩语、西班牙语、法语和德语，共 8 种语言。

文档变更须同步所有语言的安装命令、依赖要求、输出路径、反馈入口及授权说明。所有版本保留相同的语言切换顺序，图片统一引用仓库 `images/` 目录。新增语言时同步更新所有 README 的导航，并检查相对链接、图片和代码块。未经母语审校时，不声称翻译已经专业审定。

## 版本与发布

在 [CHANGELOG.md](CHANGELOG.md) 的 `Unreleased` 中记录面向用户的变化。发布准备、验证记录和版本规则见 [RELEASING.md](RELEASING.md)。

本项目采用 [MIT 许可证](LICENSE)。提交贡献时，请确认你有权按项目许可证授权该贡献；第三方内容须保留其适用许可与署名，不接受无法明确授权的第三方内容。当前状态与待核验范围见 [NOTICE.md](NOTICE.md)。

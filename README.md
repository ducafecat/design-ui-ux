# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.en.md) | 简体中文

[猫哥Flutter视频学习站](https://ducafecat.com/)

[Flutter插件站](https://flutter.ducafecat.com/)

## 安装

npx 方式安装，建议项目级别安装。

```bash
npx skills add ducafecat/design-ui-ux
```

## 使用流程

### 1、自动搜索设计方向

最好你先写一个产品的 PRD ，这样目标性强。

提示词

```bash
/design-ui-ux 编写 小红书移动端

参考
docs/prd.md
```

![自动搜索设计方向](https://files.ducafecat.com/docs/2026/11/25/1795618228981.png)

### 2、选择设计方向

如果没有你喜欢的提示词

```bash
再换一批
```

![选择设计方向](https://files.ducafecat.com/docs/2026/11/25/1795618428611.png)

### 3、设计稿落地

<img src="https://files.ducafecat.com/docs/2026/11/25/1795618786169.png" alt="提示" style="zoom: 50%;" />

提示词输入参考编号

```bash
B2
```

确认设计感觉

<img src="https://files.ducafecat.com/docs/2026/11/25/1795619134358.png" alt="设计感觉" style="zoom:50%;" />

提示词

```bash
1
```

输出 design/index.html

<img src="https://files.ducafecat.com/docs/2026/11/25/1795620741606.png" alt="设计稿落地"  />

### 4、平铺设计稿

提示词

```bash
将设计稿 design/index.html，平铺保存到 design/平铺.html
```

输出 design/平铺.html

![设计稿平铺](https://files.ducafecat.com/docs/2026/11/25/1795620965224.png)

### 5、更多玩法

可以让 AI 出 4 个首页设计稿

提示

```bash
1 2 3 4 各出一个首页设计，保存到 design/compare.html
```

输出 design/compare.html

![image-20261125231858298](https://files.ducafecat.com/docs/2026/11/25/1795619938511.png)

## 环境要求

- 安装需要 Node.js 22.20 或更高版本（包含 npm / npx）；最终 HTML 成品不需要 Node.js。
- 本地数据检索使用 Python 3，仅依赖标准库；无 Python 时可沿用详细规范，但不能声称完成检索。
- 完整设计流程需要浏览器、真实截图和本地 HTML 预览能力；默认优先 Ego Lite，需另行配置 `ego-browser` 技能。不可用时按技能规则说明并使用替代浏览器。
- 制作阶段需要可编译 Tailwind 的工具；最终成品应不依赖 Node.js、CDN 或运行时构建。

## 反馈、维护与许可

提交改进前阅读 [CONTRIBUTING.md](CONTRIBUTING.md)，版本记录见 [CHANGELOG.md](CHANGELOG.md)，敏感问题见 [SECURITY.md](SECURITY.md)。通过 [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues) 反馈可复现问题。

当前未指定项目许可证，不能据此认定为已授权的开源项目。发布前需由维护者确认代码与数据的来源、再分发权及许可证；数据中的来源记录不等于再分发授权。参见 [来源说明](NOTICE.md)。

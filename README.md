# Web Skills

面向 Codex 的网站制作 skill 集合。目前包含 **`website-studio`**：从模糊想法、已有网站或明确需求出发，协助完成需求梳理、视觉方向、页面制作、实际页面检查和交付。

## Website Studio 能做什么

- 理清网站的目标访客、主要动作、页面、功能、内容来源与上线目标；已有项目会先查看现状。
- 根据数据、权限、维护和托管需求选择相称的技术路线，避免为简单展示站加入不必要的后端。
- 询问喜欢的网站类型、参考网站、截图或组件效果；没有偏好时给出有区别的视觉方向。
- 把参考转成具体的布局、字体、配色、图片和交互规则，并根据项目需要参考 [Aceternity UI](https://ui.aceternity.com/components) 与 [shadcn/ui](https://ui.shadcn.com/) 等组件库。
- 制作或改版页面与真实功能，检查桌面和手机布局、主要操作、键盘使用、错误状态与资源加载。
- 交付运行或访问方法、已完成范围、验证结果和仍需处理的事项。

组件库是可选的灵感与实现来源。选用前应核对项目技术栈、依赖、许可和可访问性；不会因为参考某个组件库就自动更换框架。

## 安装与调用

将 [`skills/website-studio`](skills/website-studio/SKILL.md) 文件夹复制到 Codex 的 skills 目录，例如 Windows 上的 `%USERPROFILE%\.codex\skills\website-studio`。保持 `SKILL.md`、`references/` 和 `agents/` 的目录结构。

在 Codex 中直接说：

> 使用 `$website-studio` 帮我做一个产品官网。目标用户是……

也可以用于已有项目：

> 使用 `$website-studio` 改版当前网站。我喜欢这个参考网站的排版，但要保留现有功能。

如果只需要规划、单个页面或局部改动，skill 会根据任务缩小流程，不强制完成整站访谈。

## 文件结构

```text
skills/website-studio/
├── SKILL.md                    # 主流程与决策规则
├── agents/openai.yaml          # Codex 中的显示与默认调用信息
└── references/
    ├── design-content.md      # 视觉与内容细节
    └── build-verify.md        # 制作与验收细节
```

## 使用边界

这是指导 Codex 工作的 skill，并非独立运行的网站生成器。登录、支付、数据存储和上线等功能仍需项目代码、相应服务、配置与验证。对外发布、购买服务或修改生产数据需要相应授权；尚未实际测试或部署的结果会明确标为待验证。

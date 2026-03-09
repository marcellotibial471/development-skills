# Development Skills

简体中文 | [English](./README.md)

一个面向端到端软件交付流程的 development skills 仓库。

这个仓库把开发工作流拆成可复用的 agent skills，帮助你把一个需求逐步推进到有 spec、有 plan、有实现、有 review、有测试的完整交付流程。

## 包含的 Skills

- `spec`
- `plan`
- `implement`
- `review`
- `test`

## 安装方式

### Option A: skills.sh

通过 `skills.sh` 安装这个仓库里的单个 skill：

```bash
npx skills add https://github.com/SimpleEve/development-skills --skill spec
npx skills add https://github.com/SimpleEve/development-skills --skill plan
npx skills add https://github.com/SimpleEve/development-skills --skill implement
npx skills add https://github.com/SimpleEve/development-skills --skill review
npx skills add https://github.com/SimpleEve/development-skills --skill test
```

### Option B: Claude Code Plugin

通过 Claude Code marketplace 安装完整插件：

```bash
/plugin marketplace add SimpleEve/development-skills
/plugin install development-skills@simpleeve-development-skills
```

### Option C: Manual Install

```bash
git clone git@github.com:SimpleEve/development-skills.git
```

然后把一个或多个 skill 文件夹复制到宿主应用使用的本地 skills 目录下，并重启宿主应用。

## 建议说明

这套 skills 是从我自己项目里的内部 skills 抽象和泛化出来的。

原始版本里包含了不少和具体项目强相关的约定、约束和工作流细节，因此并不适合直接公开分享。这个仓库保留了核心方法和流程，但有意移除了项目特定假设。

更合适的使用方式是：把这套 skills 当作一个通用起点，而不是最终成品。拿到之后，建议你继续使用 AI 结合自己项目的实际情况，对其中的术语、目录约定、架构规则、开发流程和约束进行二次调整，让它更贴合你的项目环境。

## 使用示例

- “帮我给通知系统写一份 spec”
- “基于这个需求写实施计划”
- “按照 plan 开始实现”
- “根据 spec 和 plan review 这段代码”
- “给这个功能补测试并输出测试报告”

## License

MIT，见 [LICENSE](./LICENSE)。

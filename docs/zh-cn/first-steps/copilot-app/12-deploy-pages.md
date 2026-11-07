---
title: "第 12 课 - 使用 GitHub Pages 部署网站"
description: "使用 GitHub Copilot app 配置 Pages 工作流、审查拉取请求，并验证已发布的 Space Quiz。"
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

使用 GitHub Pages 部署 Space Quiz，让任何人都能访问。Copilot 可以准备工作流并引导部署，但你需要审查更改并确认网站已发布。

本课将完成以下任务：

- 请 Copilot 配置 GitHub Pages 部署。
- 合并前审查工作流和拉取请求。
- 跟进部署过程并验证已发布的网站。

## 场景

Space Quiz 已在 GitHub 仓库中，但还没有方便任何人访问的方式。使用 GitHub Pages 发布这个单文件网站，即可通过公开 URL 访问它，无需添加服务器或运行时依赖项。

## 请 Copilot 部署网站

在 `space-quiz` 的 Copilot app 会话中发送以下提示：

```plaintext
为此仓库启用 GitHub Pages。如有必要，创建一个 GitHub Actions 工作流来构建网站并将其部署到 GitHub Pages。如果仓库还没有 README，请添加一个，介绍此应用以及如何在本地运行它。根据这些更改创建拉取请求，并在必需的检查通过后合并。持续监控部署，直到部署成功，然后告诉我网站的最终 URL。如果你没有启用 Pages 或合并拉取请求的权限，请准确说明我需要批准或执行的操作。在网站实际发布之前，不要报告部署成功。
```

![三步示意图：合并 Space Quiz 拉取请求、GitHub Actions 部署运行成功（包含 Build website、Upload artifact 和 Deploy to Pages 步骤），以及在 yourname.github.io/space-quiz/ 打开的 Space Quiz](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> 此提示会要求代理创建并合并拉取请求，以及更改仓库的 Pages 设置。继续之前，请审查 diff、部署权限和 GitHub 的审批请求。

## 审查工作流并验证部署

1. 确认仅在仓库尚无 README 时才添加了 README。
2. 审查拉取请求中的更改，包括工作流的构建和部署步骤。
3. 仅在必需的拉取请求检查通过后合并。
4. 确认 GitHub Actions 部署运行成功。
5. 打开报告的 URL，确认 Space Quiz 可以正常加载。

如果代理无法启用 Pages 或合并拉取请求，请按其提供的具体说明操作。只有在部署成功且实际网站可以加载后，才将工作视为完成。

## 总结和后续步骤

你已将 Space Quiz 发布为实际网站，并自行验证了部署，而不是只依赖代理报告。接下来学习[第 13 课：回顾与后续步骤][next-lesson]。

[next-lesson]: ../13-review/

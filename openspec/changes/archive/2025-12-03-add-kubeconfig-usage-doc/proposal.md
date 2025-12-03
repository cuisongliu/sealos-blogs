## Why
Sealos 用户需要通过 kubeconfig 访问集群，但目前缺少官方中文指引，导致获取、导入和安全使用存在疑惑，增加了支持成本和误操作风险。

## What Changes
- 新增 kubeconfig 使用指南，覆盖 Sealos Desktop 与 CLI 获取、下载、导入的完整步骤
- 说明如何在本地使用 kubectl/helm/k9s 验证连接、切换上下文与命名空间
- 补充在 CI/CD（以 GitHub Actions 为主）中安全注入 kubeconfig 的方法，提供最小权限示例工作流与缓存建议
- 覆盖在 Sealos App Launchpad 场景中使用 kubeconfig 的指南，包括凭据挂载、上下文选择与常见操作
- 提供 GitHub Actions 通过 Launchpad API（POST /api/v1/app）管理应用的示例，说明凭据注入和最小权限
- 补充安全与权限注意事项，包括有效期、权限范围、吊销或旋转流程
- 提供常见问题与排查步骤，并在 README/导航中添加入口

## Impact
- Affected specs: kubeconfig-usage-docs（新增）
- Affected docs: 新增 kubeconfig 使用指南页面，并在首页/导航处增加入口
- 用户影响: 降低接入门槛、减少误操作和运维支持成本

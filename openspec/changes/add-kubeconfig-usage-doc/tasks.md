## 1. Implementation
- [x] 1.1 创建 kubeconfig 使用指南文档（如 `docs/kubeconfig-usage.md`），包含目录与示例命令
- [x] 1.2 说明通过 Sealos Desktop 与 CLI 获取、下载、导入 kubeconfig 的步骤，并标注上下文/命名空间范围
- [x] 1.3 展示在本地使用 kubectl/helm/k9s 配置和验证 kubeconfig 的方法（含常用命令与输出示例）
- [x] 1.4 追加 CI/CD 场景（以 GitHub Actions 为主）的使用示例，包含凭据注入、secrets 管理、最小权限示例工作流与缓存策略
- [x] 1.5 说明在 Sealos App Launchpad 中使用 kubeconfig 的方法（凭据挂载、上下文选择、应用部署常见操作）
- [x] 1.6 补充安全注意事项：权限最小化、有效期、吊销与旋转处理，以及凭据丢失的应对
- [x] 1.7 添加常见问题与排查（证书过期、无权限、网络连通性），给出可操作的检查步骤
- [x] 1.8 在 README 或文档索引处添加 kubeconfig 指南的入口链接，确保易发现

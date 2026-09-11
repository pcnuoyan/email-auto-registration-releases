# 提交与发布规则

本仓库是 iCloud HME 管理平台的公开稳定版本清单，只接受不含源码和敏感数据的版本说明更新。

## 权限边界

- `main` 的直接发布权限仅由仓库所有者 `@pcnuoyan` 持有。
- 外部用户可以提交 Pull Request，但不能直接修改仓库内容。
- 所有 Pull Request 必须由 Code Owner `@pcnuoyan` 审核批准后才能合并。
- 禁止强制推送、删除受保护分支或提交非线性历史。

## 发布内容

- 先在源码仓库完成版本验证、提交和稳定版 Tag，再更新本仓库。
- 每个版本必须新增 `releases/vX.Y.Z.md`，并在确认版本可部署后更新 `manifest.json`。
- `manifest.json` 的 `latest_version`、`release_notes_url` 和 `published_at` 必须同步更新。
- 禁止提交 CK、Cookie、密码、令牌、验证码、完整邮件、内部日志、私有源码或未修复漏洞细节。

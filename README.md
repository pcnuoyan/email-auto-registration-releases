# iCloud HME 版本信息

本仓库公开提供 iCloud HME 管理平台的稳定版本清单和用户可见更新说明，不包含应用源码、部署密钥、账户信息或内部日志。

## 文件

- [`manifest.json`](./manifest.json)：应用检查新版本时读取的稳定通道清单。
- [`releases/`](./releases)：各版本公开更新说明。

## 发布规则

- 版本号遵循语义化版本，Git tag 使用 `v` 前缀。
- `latest_version` 只指向已经完成验证、可以部署的稳定版本。
- 应用只检查并展示新版本，不从该仓库下载或自动执行更新。
- Docker 更新继续由管理员在部署宿主机上完成。
- `main` 受保护，外部提交必须通过 Pull Request 并由 Code Owner `@pcnuoyan` 批准；详细规则见 [`CONTRIBUTING.md`](./CONTRIBUTING.md)。

## 安全边界

禁止提交 CK、IMAP 密码、访问令牌、数据库连接信息、完整邮件、验证码、内部日志、私有源码地址或未修复漏洞细节。

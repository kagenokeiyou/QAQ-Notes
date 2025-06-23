# SSH

安全外壳协议（Secure Shell Protocol，简称SSH）是一种加密的网络传输协议，可在不安全的网络中为网络服务提供安全的传输环境。

## 原理

略。。。

## 基本使用

远程登录

```bash
ssh user@host
```

## 参考

### Github SSH

生成或使用现有密钥

```bash
ssh-keygen -t ed25519 -C "email@example.com"
```

将公钥 `id_ed25519.pub` 添加到 Github 的 SSH 设置中
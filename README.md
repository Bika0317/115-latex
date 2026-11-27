# 1151-Latex

115-1 專業排版與設計

[產生新的 SSH 金鑰並將其新增至 ssh-agent](https://docs.github.com/zh/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

## 建立金鑰指令

```powershell
ssh-keygen -t ed25519 -C "你的 GitHub Email"
```

## 測試 GitHub SSH 連線

```powershell
ssh -T git@github.com
```

第一次連線時，核對 GitHub 官方主機指紋，確認一致後輸入 `yes`，SSH 就會把主機金鑰記錄到 `known_hosts`。

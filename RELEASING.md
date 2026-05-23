# Releasing

这个文件记录 FlowGate 的发布流程。

## 发布前检查

1. 确认 `README.md`、`LICENSE`、`THIRD_PARTY_NOTICES.md` 已更新
2. 确认 `manifest.json`、侧边栏标题、版本展示和发布文案一致
3. 检查默认配置里没有真实密钥、手机号、邮箱、Cookie 或回调地址
4. 确认 `docs/images` 中的截图仍能正常显示
5. 复查 `git diff`，确认没有把无关临时文件带进去

## 当前版本

- 当前版本：`v1.0.0`
- 扩展版本号：`1.0.0`
- Release 文案：`docs/releases/v1.0.0.md`
- GitHub Release 正文可直接复制 `docs/releases/v1.0.0.md`

## 首次推送

```powershell
git status
git add .
git commit -m "Initial FlowGate release"
git branch -M main
git remote remove origin
git remote add origin https://github.com/a519592965/FlowGate.git
git push -u origin main
```

## 正式发布

```powershell
git status
git add manifest.json sidepanel/sidepanel.html sidepanel/update-service.js sidepanel/sidepanel.js docs/releases/v1.0.0.md RELEASING.md
git commit -m "Prepare v1.0.0 release"
git tag -a v1.0.0 -m "FlowGate v1.0.0"
git push origin main
git push origin v1.0.0
```

## Release 文案建议

- 本次版本的核心变化
- 配置和代理行为的调整
- 已知限制
- 需要用户自行准备的外部服务
- 来源说明与许可证信息

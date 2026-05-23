# FlowGate

FlowGate 1.0.3 是一个用于自动化多步骤注册与支付流程的浏览器扩展，侧重把代理、邮箱、验证码和支付链路统一到一个侧边栏里管理。

## 功能

- 自动注册 Free 账号
- 支持 Plus 支付流程
- 支持 Hotmail / Outlook、iCloud、QQ、Cloud Mail 等邮箱通道
- 支持 PayPal、GoPay 和支付转换代理
- 支持导出 / 导入配置
- 支持本地与云端的流程接入

## 使用

1. 下载并解压扩展包
2. 在 Chrome 打开 `chrome://extensions/`
3. 开启开发者模式并加载解压后的目录
4. 按界面填写代理、邮箱和流程参数

## 配置说明

- 账户接入策略建议优先使用 `SESSION JSON 导入`
- 支付转换代理仅在支付链路中生效
- 流程页面代理会贯穿整个流程，除云端支付链接外保持不变

## 版本

- 当前版本：`1.0.3`
- 发布页：`https://github.com/a519592965/FlowGate/releases`

## 项目来源

本项目基于 [QLHazyCoder/FlowPilot](https://github.com/QLHazyCoder/FlowPilot) 演进而来，并参考了 [whwh1233/StepFlow-Duck](https://github.com/whwh1233/StepFlow-Duck) 的早期链路。

原始开源项目均采用 MIT License 发布；本仓库保留相应来源与许可信息，同时对流程、配置和文案做了重新整理。

# auto-evaluate-bigc
北京印刷学院自动评教脚本 — 基于 XTmai/autoPJ 适配开发
# 🎯 北京印刷学院自动评教脚本

[![Tampermonkey](https://img.shields.io/badge/Tampermonkey-4.18+-blue.svg)](https://www.tampermonkey.net/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-4.4-orange.svg)](CHANGELOG.md)

> 北京印刷学院教务系统自动评教脚本 — 基于 [XTmai/autoPJ](https://github.com/XTmai/autoPJ) 项目适配开发

## 🙏 致谢与参考

本脚本基于 **[XTmai/autoPJ](https://github.com/XTmai/autoPJ)** 项目进行二次适配开发，感谢原作者 [XTmai](https://github.com/XTmai) 的杰出工作！

原项目地址：[https://github.com/XTmai/autoPJ](https://github.com/XTmai/autoPJ)

### 参考内容
- 核心评教逻辑框架
- Apple 风格 UI 设计理念
- Tampermonkey API 使用方式
- 进度追踪与悬浮球交互方案

### 本项目的适配与改进
- 🏫 适配北京印刷学院教务系统页面结构
- 🎲 新增随机选项功能（一道题选良好，其余选优秀）
- 🔄 优化页面跳转检测与自动重试机制
- 📝 简化评语输入（单文本框适配）

---

## 💡 项目定位

**我只是做了个适配**，让这个优秀的脚本能在北京印刷学院正常运行。

核心逻辑和 UI 框架都来自 `XTmai/autoPJ` 项目，我主要做了：
1. 修改页面选择器以匹配北京印刷学院的 HTML 结构
2. 适配 jqGrid 表格的数据读取方式
3. 测试并调整了提交流程

如果你追求**更高效、更智能**的评教体验，欢迎在此基础上进行修改和优化！本项目只是起点，期待大家贡献更多功能。

---

## ✨ 功能特点

- 🎨 **Apple 风格界面** — 毛玻璃效果，流畅动画
- 🤖 **全自动评教** — 一键开始，自动遍历所有课程
- 🎲 **智能选项** — 随机选择一道题选"良好"(80分)，其余选"优秀"(100分)
- 📝 **自定义评语** — 支持自定义评语内容
- ⚡ **快速模式** — 跳过倒计时，一键提交
- 🎯 **进度追踪** — 悬浮球实时显示完成进度
- 📋 **错误日志** — 自动记录错误，方便排查

---

## 📦 安装方法

### 方法一：直接安装（推荐）

1. 安装 [Tampermonkey](https://www.tampermonkey.net/) 浏览器扩展
2. 点击 [这里](https://github.com/你的用户名/auto-evaluate-bigc/raw/main/auto-evaluate.user.js) 安装脚本
3. 打开北京印刷学院教务系统 → 学生评价

### 方法二：手动创建

1. 打开 Tampermonkey 管理面板
2. 点击「添加新脚本」
3. 复制 `auto-evaluate.user.js` 全部内容
4. 保存（Ctrl+S）

---

## 🚀 使用指南

1. 登录北京印刷学院教务系统
2. 进入「教学评价」→「学生评价」页面
3. 页面右下角会出现蓝色悬浮球 📋
4. 点击悬浮球展开控制面板
5. 打开「自动提交」开关
6. 点击「开始评教」

---

## ⚙️ 设置选项

| 选项 | 说明 |
|------|------|
| 评语内容 | 自定义评语（500字以内） |
| 评教速度 | 提交前等待时间（1-10秒） |
| 快速模式 | 跳过倒计时，直接提交 |

---

## 🎯 适用页面

| 页面 | URL |
|------|-----|
| 评教列表 | `https://jwglxt.bigc.edu.cn/jwglxt/xspjgl/xspj_cxXspjIndex.html` |
| 评教页面 | 自动适配 |

---

## 🛠️ 开发调试

### 测试后门

双击控制面板右上角的「设置」按钮（⚙️），进入调试工具：

- 🔔 测试通知
- 🎉 测试庆祝特效
- 📋 查看错误日志

---

## 📝 更新日志

详见 [CHANGELOG.md](CHANGELOG.md)

---

## 🤝 贡献与改进

**这是你的机会！** 如果你觉得还有改进空间，欢迎 Fork 本项目并提交 PR。

### 可能的改进方向
- 🔄 更智能的选项选择策略（如根据课程类型选择不同评分）
- 📊 批量操作优化，进一步提升速度
- 🎨 更多主题风格切换
- 🌐 适配更多院校的教务系统
- 📱 移动端适配优化

### 贡献方式
1. Fork 本项目
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的修改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

---

## ⚠️ 免责声明

- 本脚本仅供学习交流使用
- 请合理使用，不得用于恶意目的
- 使用本脚本产生的一切后果由使用者承担
- 请遵守北京印刷学院的相关规定

---

## 📄 开源协议

MIT License

---

**⭐ 如果觉得有用，请给个 Star！你的支持是我继续维护的动力！**

**🔧 如果你想改进它，Fork 并 PR！让我们一起让它变得更好！**

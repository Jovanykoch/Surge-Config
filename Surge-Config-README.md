# 🚀 Surge-Config

> 🌐 高质量、模块化的 Surge 配置文件合集 —— 简洁、清晰、可扩展。

## 📖 简介

**Surge-Config** 是一套适用于 **Surge for iOS / macOS** 的网络代理配置文件集合，包含分流规则、模块脚本以及推荐策略组设置。  
旨在帮助用户快速部署稳定、整洁的 Surge 网络环境。

## 🧩 功能特点

- 🧱 **模块化设计** — 各功能独立拆分，按需引入  
- 🚀 **优化规则集** — 合并常见分流规则、广告过滤、流媒体分流  
- 🧰 **可维护性高** — 目录清晰、注释完整，方便长期维护  
- 🌍 **兼容多平台** — 适配 Surge iOS / macOS（建议版本 ≥ 5.0）  
- 🔁 **自动更新可拓展** — 支持通过脚本或 GitHub Actions 自动更新  

---

## 📂 目录结构

```
Surge-Config/
├── README.md                # 项目说明文档
├── LICENSE                  # 授权协议（建议 MIT）
├── profiles/                # 完整的配置模板
│   ├── default.conf
│   └── minimal.conf
├── rules/                   # 各类分流与屏蔽规则
│   ├── adblock.list
│   ├── global.list
│   └── streaming.list
├── modules/                 # Surge 模块文件（.sgmodule）
│   ├── YouTube.sgmodule
│   ├── Telegram.sgmodule
│   └── Custom.sgmodule
└── scripts/                 # 自动化脚本
    └── update.sh
```

---

## ⚙️ 使用方法

### ✅ 方法一：直接导入配置
1. 打开 **Surge → Profiles → New Profile → From URL**
2. 粘贴仓库中某个 `.conf` 文件的原始链接，例如：
   ```
   https://raw.githubusercontent.com/jovanykoch/Surge-Config/main/profiles/default.conf
   ```
3. 点击 **Save & Apply** 即可。

### 🧩 方法二：模块化加载
1. 打开你的主配置文件（如 `Surge.conf`）
2. 在合适位置引入模块：
   ```
   [General]
   include = https://raw.githubusercontent.com/jovanykoch/Surge-Config/main/modules/YouTube.sgmodule
   ```

---

## 🧠 推荐规则分类说明

| 分类 | 功能描述 |
|------|-----------|
| `adblock.list` | 屏蔽常见广告与追踪域名 |
| `global.list` | 国际站点直连或代理规则 |
| `streaming.list` | 视频平台加速、解锁流媒体区域限制 |
| `Telegram.sgmodule` | 优化 Telegram 连接体验 |
| `YouTube.sgmodule` | 改善 YouTube 缓冲与代理策略 |

---

## 🛠️ 更新方式

### 手动更新
直接在 Surge 的 **Profiles** 页面点击 “Check for Updates”。

### 自动更新（可选）
你可以使用脚本（例如 `scripts/update.sh`）或 GitHub Actions 定期自动刷新规则文件。

---

## 📜 License

本项目推荐使用 **MIT License** 或 **CC BY 4.0** 授权。  
你可以自由复制、修改、分发，但请保留作者署名。

---

## 💬 致谢

感谢以下开源项目与规则提供者（如有引用请补充）：  
- [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR)  
- [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script)  
- [ConnersHua/Profiles](https://github.com/ConnersHua/Profiles)

---

## 🧑‍💻 作者信息

**Author:** [@jovanykoch](https://github.com/jovanykoch)  
**Project:** [Surge-Config](https://github.com/jovanykoch/Surge-Config)  
**Last Update:** 2025-10-27  

---

## 🌟 支持项目

如果这个项目对你有帮助，可以：
- ⭐ **Star** 支持一下  
- 或 **Fork** 一份进行自定义修改  

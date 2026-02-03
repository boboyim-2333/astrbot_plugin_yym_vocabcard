# AstrBot 每日单词卡片插件
> 喜欢的话可以给个 Star 喵，有问题欢迎提 Issue/PR
<div align="center">

📚 每日多语种单词卡片推送插件 - 玻璃拟态风格

[![License](https://img.shields.io/badge/license-AGPL--3.0-blue.svg)](LICENSE)
[![AstrBot](https://img.shields.io/badge/AstrBot-Plugin-orange.svg)](https://github.com/Soulter/AstrBot)

</div>

## 📸 效果预览

<div align="center">
<img src="example.png" width="300" alt="卡片效果"/>
</div>

> 玻璃拟态风格卡片，分辨率 **1728 × 2160 像素**

## 🎮 快速上手

| 命令 | 说明 |
|------|------|
| `/vocab` | 立即获取一张单词卡片 |
| `/vocab_lang [语种ID]` | 切换卡组（不带参数显示列表） |
| `/vocab_status` | 查看学习进度 |
| `/vocab_register` | 注册每日推送 |
| `/vocab_unregister` | 取消每日推送 |
| `/vocab_help` | 显示帮助 |

## 📚 支持的卡组

| 卡组 | 词条数 | 说明 |
|------|--------|------|
| english | 3,722 | 英语六级核心词汇 |
| japanese | 10,147 | 日语JLPT N1-N5（支持等级筛选） |
| idiom | 824 | 常用成语 |
| classical | 27 | 古文经典句子 |
| radio | 361 | 无线电法规题库 |

## 📦 安装

### 1. 克隆插件

```bash
cd addons/plugins/
git clone https://github.com/itismygo/astrbot_plugin_vocabcard.git
```

### 2. 安装依赖

```bash
pip install -r requirements.txt
```

> 首次生成卡片时会自动下载 Chromium 浏览器（约 150MB）

### 3. 重启 AstrBot

## ⚙️ 主要配置

| 配置项 | 说明 | 默认值 |
|--------|------|--------|
| current_language | 当前卡组 | english |
| japanese_level | 日语等级筛选 | all |
| push_time_generate | 卡片生成时间 | 07:30 |
| push_time_send | 推送时间 | 08:00 |
| learning_mode | 学习模式 | random |

## 🐛 常见问题

**Q: 首次使用较慢？**
> 首次运行会自动下载 Chromium 浏览器，请耐心等待

**Q: 推送不生效？**
> 1. 检查是否已使用 `/vocab_register` 注册
> 2. 检查推送时间配置

**Q: 清空学习进度？**
> 删除 `data/progress_<语种>.json` 文件

## 📄 许可证

AGPL-3.0 License

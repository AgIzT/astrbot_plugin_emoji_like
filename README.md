
<div align="center">

![:name](https://count.getloli.com/@astrbot_plugin_emoji_like?name=astrbot_plugin_emoji_like&theme=minecraft&padding=6&offset=0&align=top&scale=1&pixelated=1&darkmode=auto)

# astrbot_plugin_emoji_like

_✨ 智能贴表情 ✨_  

[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![AstrBot](https://img.shields.io/badge/AstrBot-3.4%2B-orange.svg)](https://github.com/Soulter/AstrBot)
[![GitHub](https://img.shields.io/badge/作者-Zhalslar-blue)](https://github.com/Zhalslar)

</div>

## 🤝 介绍

调用 LLM 判断消息情感，并根据情绪给 QQ 消息贴上合适的表情反应。

新版主动贴表情不再对所有普通群消息随机触发，而是仅在用户明确触发 Bot 回复时，按配置概率给触发者的那条消息贴 1 个表情。

## 📦 安装

在 AstrBot 的插件市场搜索 `astrbot_plugin_emoji_like`，点击安装即可。

## ✨ 功能

- 被 @、被回复、或消息包含配置关键词时，按概率给触发者消息贴表情
- 使用 LLM 判断文本/图片消息情绪，并映射到对应 QQ 表情 ID
- 支持回复消息后使用 `贴表情 <数量>` 手动贴表情
- 支持跟随群友消息中已有的 QQ 表情
- 支持跟随群友给消息添加的表情反应

## ⌨️ 使用说明

### 触发方式

| 触发方式 | 说明 |
|:--:|:--|
| @Bot / AstrBot 唤醒命令 | 按 `emoji_like_prob` 概率给触发者消息贴 1 个表情 |
| 回复 Bot 的消息 | 按 `emoji_like_prob` 概率给触发者消息贴 1 个表情 |
| 包含关键词的群消息 | 关键词由 `emoji_like_trigger_keywords` 配置，适合填写 Bot 名字、昵称或唤醒词 |
| 回复消息后发送 `贴表情 <数量>` | 手动给被回复消息贴表情；不填数量时默认贴 5 个 |

普通群消息不会再随机触发主动情绪贴表情。如需让“提到 Bot 名字”也触发，可在配置中的 `emoji_like_trigger_keywords` 填写 Bot 名字、昵称或唤醒词。

### 常用配置

| 配置项 | 说明 |
|:--|:--|
| `emoji_like_prob` | 触发 Bot 回复时，给触发者消息贴表情的概率 |
| `emoji_like_trigger_keywords` | 触发表情贴贴的关键词列表，支持包含匹配 |
| `emoji_follow_prob` | 群友消息中含 QQ 表情时，Bot 跟随贴同类表情的概率 |
| `reaction_follow_enabled` | 是否跟随群友添加的表情反应 |
| `reaction_follow_prob` | 跟随群友表情反应的概率 |
| `judge_provider_id` | 判断情感使用的 LLM 提供商 |
| `emotions_mapping_list` | 情感关键词到 QQ 表情 ID 的映射表 |

### 示例图

![download](https://github.com/user-attachments/assets/22d4a258-1d84-430e-9832-de2b12cdd9cf)

## 👥 贡献指南

- 🌟 Star 这个项目！（点右上角的星星，感谢支持！）
- 🐛 提交 Issue 报告问题
- 💡 提出新功能建议
- 🔧 提交 Pull Request 改进代码

## 📌 注意事项

- 想第一时间得到反馈的可以来作者的插件反馈群（QQ群）：460973561（不点star不给进）

<a href="https://t.me/NewRSSBbot"><img width="150" height="150" align="left" style="float: left; margin: 0 10px 0 0;" alt="newRSSBot icon" src="docs/resources/newRSSBot_icon.svg"/><a/>

# [RSS to Telegram Bot](https://t.me/NewRSSBbot)

**关心你的阅读体验的 Telegram RSS 机器人**


[![GitHub last commit (dev)](https://img.shields.io/github/last-commit/Jv0id/RSS-to-Telegram-Bot/dev?logo=github)](https://github.com/Jv0id/RSS-to-Telegram-Bot/commits/dev)
[![Translating status](https://img.shields.io/weblate/progress/rss-to-telegram-bot?logo=weblate&color=informational)](https://hosted.weblate.org/engage/rss-to-telegram-bot/)
[![GitHub stars](https://img.shields.io/github/stars/Jv0id/Rss-to-Telegram-Bot?style=social)](https://github.com/Jv0id/RSS-to-Telegram-Bot/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Jv0id/RSS-to-Telegram-Bot?style=social)](https://github.com/Jv0id/RSS-to-Telegram-Bot/fork)

[![Telegram bot](https://img.shields.io/badge/bot-%40RSStT__Bot-229ed9?logo=telegram&style=for-the-badge)](https://t.me/NewRSSBbot)

# 欢迎加入telegram [有声小说频道](https://t.me/youshenggushi) [![Telegram](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.swo.moe%2Fstats%2Ftelegram%2Fyoushenggushi&query=count&color=2CA5E0&label=Telegram&labelColor=282c34&logo=telegram&suffix=+members&cacheSeconds=3600)](https://t.me/youshenggushi)

|  [更新日志]  | [FAQ] |  [文档]  | [使用 RSS_BOT 的频道] |
|:--------:|-------|:------:|:--------------:|

[更新日志]: docs/CHANGELOG.zh.md

[FAQ]: docs/FAQ.zh.md

[文档]: docs

[使用 RSS_BOT 的频道]: docs/channels-using-rsstt.md

## 亮点

- 多用户
- 国际化
    - 英语、中文、粤语、意大利语还有[更多](docs/translation-guide.md)！
- RSS 源的文章内容可被发送至 Telegram
    - 保持富文本格式
    - 保持媒体文件 (可自定义)
        - 在文章内容或者 enclosure 里的图片、视频、音频；和在文章 enclosure 里的文档
        - 长图会作为文件发送，防止 Telegram 将它压缩得不可读
        - 丢弃烦人的图标，它们破坏了阅读体验
    - 自动替换 emoji shortcodes 为 emoji
    - 自动替换满足某些特征的表情图片为 emoji 或其描述文本
    - 自动判断 RSS 源的标题是否为自动填充，并自动选择是否略去标题 (可自定义)
    - 自动显示作者名 (可自定义)
    - 自动切分超长消息
        - 如果配置了 Telegraph，消息会通过 Telegraph 发出 (可自定义)
- [丰富的自定义格式设定](docs/formatting-settings.md)
    - Hashtag、自定义标题，等等
- 为 Telegram 和 RSS 源配置独立的代理设置
- OPML 导入和导出 (保持自定义标题)
- 自定义订阅
- 优化的性能 (参见 [FAQ](docs/FAQ.zh.md#q-bot-的性能怎么样))
- 用户友好
- HTTP 缓存

## 部署

[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rsstt?logo=python&label=&labelColor=white)](https://www.python.org)
[![Docker Image Size (tag)](https://img.shields.io/docker/image-size/jp0id/rss-to-telegram/latest?logo=docker)](https://hub.docker.com/r/jp0id/rss-to-telegram)
[![Docker pulls](https://img.shields.io/docker/pulls/jp0id/rss-to-telegram?label=pulls&logo=docker&color=informational)](https://hub.docker.com/r/jp0id/rss-to-telegram)

部署 RSS_BOT 实例非常简单。最推荐的部署方式是 Docker Compose: 它适合几乎所有 VPS。[Railway.app](https://railway.app) (一个 PaaS 平台) 也得到了官方支持。您也可以使用 pip 从 PyPI (跟踪 `master` 分支) 或 TestPyPI (跟踪最新的 `dev` 分支) 安装 RSS_BOT。对于开发人员或有经验的用户，从源代码直接运行也是一个选项。

<a href="docs/deployment-guide.md#option-2-railwayapp"><img src="https://railway.app/button.svg" height="30" alt="Deploy on Railway"></a>

详情请参阅[部署指南](docs/deployment-guide.md)。

## 翻译

在[这里](docs/translation-guide.md)阅读翻译指南。

你可以通过 [Hosted Weblate](https://hosted.weblate.org/projects/rss-to-telegram-bot/) 帮助翻译这个 bot。特别感谢他们为自由项目提供的免费托管服务！

<a href="https://hosted.weblate.org/engage/rss-to-telegram-bot/"><img src="https://hosted.weblate.org/widgets/rss-to-telegram-bot/zh_Hans/glossary/multi-auto.svg" width = "500" alt="" /></a>

## 使用公共 bot

[公共 bot](https://t.me/NewRSSBbot) 没有服务保障。我会尽我所能维护它，但不能保证它永远完美运作。同时，你应该遵循“公平使用”，避免订阅过多 RSS 源。  
如果你在频道里使用[公共 bot](https://t.me/NewRSSBbot) ，请考虑在频道简介 (或置顶消息) 里提及这个 bot (或这个项目)，来让更多人了解本项目。这不是强制的。

## 使用 RSS_BOT 的频道

想要预览 RSS_BOT 发送的消息的模样吗？这里有一个[使用 RSStT 的频道列表](docs/channels-using-rsstt.md)

## 许可证

本项目根据 [AGPLv3](LICENSE) 授权。严禁闭源的分发或机器人托管。如果你修改了代码并分发或托管它，请确保任何可以使用你的 bot 的用户都可以获得源代码 (通过在 [`src/i18n/__init__.py`](src/i18n/__init__.py) 中编辑仓库 URL)。

本仓库原是 [Rongronggg9/RSS-to-Telegram-Bot](https://github.com/Rongronggg9/RSS-to-Telegram-Bot) 的一个 fork。仅更改了telegraph部分布局。

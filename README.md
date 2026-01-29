# 👁️ Yongmai OS v2.0: 全球投资情报源清单 (indie investor's Bloomberg Terminal)

这是一个开源项目，旨在提供一套经过实战验证的、高价值的全球投资信息源清单。它是我的 **"金融外骨骼" (Yongmai OS)** 系统的“眼睛”模块，负责市场信息的雷达扫描。

正如我在视频中所说，AI 的价值在于“做以前做不到的事”。这套清单的意义在于：**将你的信息获取效率提升到以前做不到的高度。**

## 🚀 如何使用？ (Quick Start)

如果你是追求效率的极客，可以直接下载 `sources.opml` 文件，导入到你常用的 RSS 阅读器（如 Feedly, Inoreader, Reeder 等）即可一键订阅所有源。

如果你是想深入研究的架构师，请参考下方的分类表格，了解每个信息源的战略定位。

## 🎯 核心架构：信息源的战略分类

这套信息源清单并非简单堆砌，而是按照我的投资策略逻辑，被划分为三大战略模块：

| 模块 | 战略定位 | 关注重点 | 包含源数量 |
| :--- | :--- | :--- | :--- |
| **SOP 1 深度洞察 (Brain)** | 长期逻辑、商业模式、宏观定调 | 投资的 **Why** 和 **What** | 10 |
| **SOP 2 势能扫描 (Pulse)** | 资金流向、评级调整、突发热点 | 投资的 **When** 和 **Where** | 9 |
| **辅助：区域/垂类 (Auxiliary)** | 查漏补缺、特定机会、技术前沿 | 投资的 **How** 和 **Next** | 9 |

## 📋 信息源清单 (Total: 28 Sources)

| 类别 | 来源名称 | 战略价值 | URL / RSSHub 配置 |
| :--- | :--- | :--- | :--- |
| **SOP 1 深度洞察** | The Information | 美股科技深喉，商业模式分析 | `https://www.theinformation.com/feed` |
| | Stratechery | 商业模式分析天花板 | `https://stratechery.com/feed/` |
| | Bloomberg Tech | 巨头动向与科技趋势 | `https://feeds.bloomberg.com/technology/news.rss` |
| | Bloomberg Opinion (Matt Levine) | 金融深度评论，华尔街洞察 | `https://www.bloomberg.com/opinion/authors/ARbTQlRLRjE/matthew-s-levine.rss` |
| | FT Tech | 欧洲/全球科技视角 | `https://www.ft.com/technology?format=rss` |
| | Seeking Alpha Editors' Picks | 美股个股深度逻辑 | `https://seekingalpha.com/tag/editors-picks.xml` |
| | The Economist | 全球宏观定调与经济趋势 | `https://www.economist.com/finance-and-economics/rss.xml` |
| | ARK Invest | 颠覆性创新逻辑与投资方向 | `https://ark-invest.com/feed/` |
| | 东财·策略研报 | A股策略深度研究 | `rsshub搭建/eastmoney/report/strategyreport` |
| | 东财·宏观研究 | 中国宏观深度分析 | `rsshub搭建/eastmoney/report/macresearch` |
| **SOP 2 势能扫描** | MarketBeat Instant Alerts | 美股版“券商晨报”，评级和异动 | `https://www.marketbeat.com/rss/instant-alerts.xml` |
| | 金十数据·重要 | 全球宏观哨兵，突发事件 | `rsshub搭建/jin10/:important?` |
| | 金十·美股 | 美股盘前盘后动态 | `rsshub搭建/jin10/topic/424` |
| | Bloomberg Markets | 华尔街资金流向 | `https://feeds.bloomberg.com/markets/news.rss` |
| | FT Markets | 全球市场动态与交易信号 | `https://www.ft.com/markets?format=rss` |
| | 财联社·热门 | A股游资/政策风向 | `rsshub搭建/cls/hot` |
| | TechCrunch | 一级市场热点与风投动态 | `https://techcrunch.com/feed/` |
| | The Block | Crypto 机构视角与深度分析 | `rsshub搭建/theblock/category/crypto-ecosystems` |
| | Bloomberg Crypto | Crypto 主流视角与市场动态 | `https://feeds.bloomberg.com/crypto/news.rss` |
| **辅助：区域/垂类** | TechInAsia | 东南亚科技与创投 | `https://www.techinasia.com/feed` |
| | Technode | 中国科技出海与创新 | `https://technode.com/feed/` |
| | EU-Startups | 欧洲创投与科技 | `https://www.eu-startups.com/feed/` |
| | AltAssets | LP/另类资产与私募股权 | `https://www.altassets.net/feed` |
| | 东财·券商晨报 | A股券商晨报与个股推荐 | `rsshub搭建/eastmoney/report/brokerreport` |
| | MacroMicro | 宏观数据与图表分析 | `https://sc.macromicro.me/feed` |
| | Followin | Crypto 补充信息与社区热点 | `rsshub搭建/followin/1/zh-Hans` |
| | Nvidia 官方博客 | 科技巨头官方技术博客 | `https://blogs.nvidia.com/feed/` |
| | The Verge | 消费电子与产品趋势 | `https://www.theverge.com/rss/index.xml` |

## 🛠️ 进阶：从手动版到 AI 自动化

这份清单是你的 **MVP (最小可行性产品)**。如果你想追求极致的自动化，请参考我在视频中提到的进阶路径：

1.  **非标信息标准化**：使用 **RSSHub** https://docs.rsshub.app/deploy/ 搭建服务，将非 RSS 格式的网站（如东财研报、金十数据）转化为标准的 RSS 格式。
2.  **数据清洗与调度**：使用 **WordPress 插件** 或 **AI 编程**（如 Python + BeautifulSoup/Requests）进行抓取和初步清洗。
3.  **AI Agent 编排**：将清洗后的数据作为 Agent 的输入，实现自动巡逻、自动审计和自动报告生成。

**免责声明：** 本清单仅供学习和研究使用，不构成任何投资建议。请根据您的投资策略和风险承受能力谨慎使用。

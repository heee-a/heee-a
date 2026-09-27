# 你好，我是 heee-a 👋

**数据分析 · 数据工程 · 后端开发 · AI 应用** 方向。这个账号是一个
有纪律的开源作品集：**9 个仓库、20+ 子项目、190+ 自动化测试、全部 CI 通过**；
数据项目使用真实公开数据采集，所有结论可由仓库内脚本一键复现。

> Data analysis / data engineering / backend / AI applications.
> 9 repos, 20+ sub-projects, 190+ automated tests, every number reproducible.

## 📂 作品集导览（按方向）

### 📊 数据分析
| 仓库 | 亮点 |
|---|---|
| [**data-portfolio**](https://github.com/heee-a/data-portfolio) | 9 个采集→清洗→分析→结论全链路项目：17 城气象（39,456 天零缺失）、GitHub 仓库画像、世界指标面板、SQL、统计推断、文本挖掘、时序预测、双爬虫 |
| [**bda-toolkit**](https://github.com/heee-a/bda-toolkit) | pip 可装的商用分析工具箱：RFM / ABC / 留存 / 购物篮 / 漏斗，一条命令 16 Sheet 报告 |

### 🏭 数据工程
| 仓库 | 亮点 |
|---|---|
| [**dataforge**](https://github.com/heee-a/dataforge) | ETL 实战：水位线增量采集 → SQLite 星型数仓 → 质量门禁（error/warn 规则引擎）→ 自动日报；幂等性实测验证 |

### 🧠 机器学习与 AI
| 仓库 | 亮点 |
|---|---|
| [**ml-bench**](https://github.com/heee-a/ml-bench) | 多模型基准（最高 98.3%）+ Wilcoxon 显著性检验、标签泄漏对照实验、A/B 测试蒙特卡洛互证、学习曲线 |
| [**ai-lab**](https://github.com/heee-a/ai-lab) | BM25 检索问答（recall@3 83% 含评测演进）、手写 CART 决策树、PyTorch 对照实验（诚实负结果）、自包含仪表盘 |
| [dev-portfolio/ai-agents](https://github.com/heee-a/dev-portfolio/tree/main/ai-agents) | 从零实现 ReAct 智能体框架：工具沙箱、自我纠错循环、任意 OpenAI 兼容模型可接 |

### 💻 软件开发与算法
| 仓库 | 亮点 |
|---|---|
| [**dev-portfolio**](https://github.com/heee-a/dev-portfolio) | 5 类别 11 子项目：FastAPI 分层后端、10 个设计模式、JSON 解析器、三种限流器、cron 调度器、表达式语言（Pratt 解析）、TUI 仪表盘、异步采集（实测 3.6×）、25+ 算法与性能基准 |

### 🎮 垂直应用
| 仓库 | 亮点 |
|---|---|
| [**yanyun-gradecalc**](https://github.com/heee-a/yanyun-gradecalc) | OCR Web 应用：斜拍照片词条配对算法 100% 准确，多方案本地管理，公开可用 |
| [**windsmeet-tools**](https://github.com/heee-a/windsmeet-tools) | 游戏资源建模：心力/体力模拟与养成规划器 |

## 🖼 作品速览

| ![六城月均温](https://raw.githubusercontent.com/heee-a/data-portfolio/main/projects/01_weather_cities/charts/monthly_temp.png) | ![Preston曲线](https://raw.githubusercontent.com/heee-a/data-portfolio/main/projects/03_world_indicators/charts/income_life.png) |
|---|---|
| [城市气象](https://github.com/heee-a/data-portfolio/tree/main/projects/01_weather_cities)：南北冬差 37℃ vs 夏差 13℃ | [世界指标](https://github.com/heee-a/data-portfolio/tree/main/projects/03_world_indicators)：收入-寿命 Preston 曲线 |
| ![泄漏对照](https://raw.githubusercontent.com/heee-a/ai-lab/main/projects/01_ml_pipeline/charts/leakage.png) | ![功效曲线](https://raw.githubusercontent.com/heee-a/ml-bench/main/projects/05_ab_simulation/charts/power_curve.png) |
| [ai-lab · 泄漏对照实验](https://github.com/heee-a/ai-lab/tree/main/projects/01_ml_pipeline)：答案喂进特征 +10pp | [ml-bench · A/B 方法论](https://github.com/heee-a/ml-bench/tree/main/projects/05_ab_simulation)：功效曲线蒙特卡洛互证 |

## 🛠️ 技术栈

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white)
![matplotlib](https://img.shields.io/badge/matplotlib-11557C?logo=matplotlib&logoColor=white)
![plotly](https://img.shields.io/badge/plotly-239120?logo=plotly&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)

## ✨ 作品集的三条原则

1. **真实** — 所有数据来自公开 API/站点的真实采集（World Bank / GitHub /
   Open-Meteo / CAMS / toscrape…），所有指标由仓库脚本实测生成；
2. **可复现** — 每个项目 `python xxx.py` 一键跑通，数据快照随仓库提供，
   CI 在三个 Python 版本上自动验证；
3. **诚实** — 不显著的检验、被数据推翻的预设叙事、MAPE 在零附近的爆炸、
   深度模型输给 SVM 的负结果——都原文保留。工程判断比漂亮数字更重要。

## 📄 文档

- [RESUME.md](RESUME.md) — 简历呈现：可直接粘贴的项目经历条目 + 按岗位选配建议
- [INTERVIEW.md](INTERVIEW.md) — 面试讲稿：10 个项目的 STAR 讲稿与追问预案

## 🕘 更新日志

| 日期 | 内容 |
|---|---|
| 2026-09 中 | 新增 dataforge 数据管道实战（增量/幂等/质量门禁/日报） |
| 2026-09 中 | dev-portfolio 扩至 5 类别 11 子项目（+JSON 解析器、限流器） |
| 2026-09 中 | ml-bench +A/B 方法论、学习曲线；ai-lab +决策树从零、PyTorch 对照 |
| 2026-09 上 | data-portfolio +HTML 爬虫（books/quotes 双沙盒）；yanyun-gradecalc Web 化 |
| 2026-09 初 | 首批 4 仓库上线（data-portfolio / bda-toolkit / windsmeet-tools / yanyun-gradecalc） |

## 📈 关注方向

时序预测 · 检索增强生成（RAG）· 数据管道编排 · 因果推断

---
<!--heee-a/data-portfolio 是数据方向主作品集；heee-a/dev-portfolio 是开发方向主作品集-->

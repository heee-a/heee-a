# 简历呈现指南 · 可直接粘贴的项目经历

> 本文档把 9 个仓库提炼成简历可用的文字。所有数字均来自各仓库实测，
> 面试被追问时可现场打开仓库复现。**只写你能讲深的项目**——每个条目
> 后面都标注了对应的追问预案位置（INTERVIEW.md）。

## 一、简历上的 GitHub 链接怎么放

1. **联系方式区**：`GitHub：github.com/heee-a`（作品集入口，主页有导览）；
2. **项目经历区**：每个项目标题后附具体仓库链接（见下方条目）；
3. 面试前在 GitHub 主页手动 **Pin（置顶）** 4 个与岗位最相关的仓库；
4. 建议（可选）：归档与作品集无关的旧仓库，保持主页整洁。

## 二、项目经历 · 完整版

### 数据采集与分析平台（data-portfolio）
`Python` `Requests` `Pandas` `Matplotlib` `SciPy` ｜ github.com/heee-a/data-portfolio

- 设计礼貌采集基座（磁盘缓存、限速、429 指数退避），从 World Bank、GitHub、
  Open-Meteo 等公开 API 采集 7 万+ 行真实数据，全程无人干预自动恢复限流
- 独立完成 8 个全链路分析项目：17 城气象（39,456 天零缺失）、GitHub 头部仓库
  画像（1000 仓库）、世界发展指标面板（217 国 × 24 年）、SQL 分析、统计推断、
  文本挖掘、时序预测、HTML 爬虫
- 建立数据质量回归测试；如实报告不显著的负结果与被数据推翻的预设结论
  （如"北方采暖更糟"的二分叙事被逐城数据证伪）

### 机器学习基准实验室（ml-bench）
`Scikit-learn` `SciPy` `Plotly` ｜ github.com/heee-a/ml-bench

- 构建 3 数据集 × 5 模型 × 10 次重复分层交叉验证基准，最高准确率 98.3%
  （手写数字）；以 Wilcoxon 配对检验证明头部模型差异不显著（p>0.2），
  避免把随机波动当成模型提升
- 设计标签泄漏对照实验：量化"将人均GDP 放入收入等级预测特征"造成的
  +10pp 准确率虚高，演示泄漏的识别、防范与口径修正过程
- 从零实现 BM25 与 TF-IDF+SVD 检索器，建立 12 题中文评测集驱动迭代
  （recall@3 50%→83%）；实测小语料场景 BM25 优于向量检索，以数据修正技术选型
- 完成 A/B 测试方法论全实现：样本量公式与 2000 次蒙特卡洛模拟互证
  （理论功效 80% vs 实测 80.5%）、A/A 假阳性率 5.3%≈α

### AI 智能体与 Web 应用（yanyun-gradecalc / dev-portfolio）
`FastAPI` `RapidOCR` `PyTorch` `asyncio` `aiohttp` ｜
github.com/heee-a/yanyun-gradecalc · github.com/heee-a/dev-portfolio

- 独立开发公开可用的 OCR 识别 Web 应用：手机斜拍照片经"数值列聚类 +
  保序动态规划配对 + 词条类型约束"算法实现 100% 词条配对；EXIF 转正 +
  四朝向旋转重试兜底横竖屏问题；照片内存处理不落盘，用户方案仅存本地浏览器
- 从零实现 ReAct 智能体框架：工具注册表（签名自动生成 JSON Schema）、
  AST 白名单安全计算器、错误观察回环自我纠正，支持任意 OpenAI 兼容模型
- asyncio 异步采集器较同步版实测 3.6× 提速（20 页 30.2s→8.4s，
  礼貌限速下的公平对比）

### 商业数据分析工具箱（bda-toolkit）
`Pandas` `Matplotlib` `OpenPyxl` ｜ github.com/heee-a/bda-toolkit

- 开发 9 大分析模块（清洗/EDA/同比环比/ABC/RFM/留存/购物篮/漏斗），
  一条命令对任意订单明细生成 16 Sheet Excel 分析报告与全部图表
- pip 可安装，内置 21 项单元测试与 GitHub Actions CI（3 个 Python 版本）

## 三、项目经历 · 精简版（简历空间有限时）

- **数据采集与分析平台**（Python）：8 个全链路项目，公开 API 采集 7 万+ 行，
  统计检验驱动结论；github.com/heee-a/data-portfolio
- **机器学习基准**（Scikit-learn）：多模型交叉验证 + 显著性检验，最高 98.3%；
  标签泄漏对照实验；github.com/heee-a/ml-bench
- **OCR 识别 Web 应用**（FastAPI/RapidOCR）：斜拍照片词条配对算法 100% 准确，
  多方案本地管理；github.com/heee-a/yanyun-gradecalc
- **ReAct 智能体框架**（Python）：工具沙箱、自我纠错循环，离线可测；
  github.com/heee-a/dev-portfolio

## 四、按岗位选配建议

| 目标岗位 | 简历主打（按顺序） | 面试深讲 |
|---|---|---|
| 数据分析 | data-portfolio → ml-bench → bda-toolkit | 统计推断、A/B、SQL 项目 |
| 数据工程 | dataforge → data-portfolio → ml-bench | 增量采集、幂等、质量门禁 |
| 后端开发 | dev-portfolio → dataforge → yanyun-gradecalc | FastAPI 分层、asyncio 并发 |
| AI 应用/算法 | ai-lab → dev-portfolio/ai-agents → ml-bench | RAG 评测、ReAct、泄漏实验 |

## 五、最终仓库清单（2026-09 核验）

| 仓库 | 内容 |
|---|---|
| github.com/heee-a/data-portfolio | 数据采集与分析（8 项目） |
| github.com/heee-a/dev-portfolio | 软件开发 / AI 智能体 / 算法（5 类别 9 子项目） |
| github.com/heee-a/ai-lab | 机器学习 / RAG / 仪表盘（4 项目） |
| github.com/heee-a/ml-bench | 机器学习基准 / 空气质量 / A/B（5 项目） |
| github.com/heee-a/bda-toolkit | 商业数据分析工具箱 |
| github.com/heee-a/yanyun-gradecalc | OCR 识别 Web 应用 |
| github.com/heee-a/windsmeet-tools | 游戏数据建模工具 |
| github.com/heee-a/dataforge | 数据管道实战（ETL） |
| github.com/heee-a | GitHub 主页（作品集导览 + 面试讲稿） |

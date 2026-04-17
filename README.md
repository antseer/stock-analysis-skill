# Stock Analysis Skill

这个仓库保存 `stock-analysis` 技能的发布包，以及一个可直接打开的可视化报告示例。

当前仓库里的核心文件：

- `stock-analysis-v4.skill`：当前发布包，文件名沿用旧版命名，但内容已更新为最新股票版技能包
- `stock-dark-report.html`：静态深色版股票分析报告示例，可直接在浏览器里打开预览
- `skill.meta.json`：给 Antseer Skillhub 使用的结构化技能元数据
- `README.md`：仓库说明

## 当前发布内容

这次同步后的技能包版本为 `v6.5.0`，聚焦于美股分析，不再包含加密货币相关描述或能力说明。当前对外展示的核心能力包括：

- 美股 8 维打分与 7 档评级
- 多股票批量并行分析与相对排名
- 内置预置股票目录，可直接返回常见股票清单
- `--catalog` / `/stock_catalog` 快速输出股票目录 JSON
- ticker 自动规范化，例如 `BRK.B` -> `BRK-B`
- 输出中支持展示中文股票名
- 数据完整度提示与失败原因分类
- 股息分析
- 自选股与提醒
- 投资组合管理
- Hot Scanner 热点扫描
- Rumor Scanner 早期信号/传闻扫描
- HTML / Markdown / JSON / Text 多格式输出

## 仓库内容说明

`stock-analysis-v4.skill` 是一个 zip archive，包内包含：

- `SKILL.md`
- `README.md`
- `docs/`
- `scripts/analyze_stock.py`
- `scripts/hot_scanner.py`
- `scripts/rumor_scanner.py`
- `scripts/dividends.py`
- `scripts/portfolio.py`
- `scripts/watchlist.py`
- `scripts/test_stock_analysis.py`

## 使用方式

直接预览报告示例：

```bash
open stock-dark-report.html
```

查看技能包内容：

```bash
unzip -l stock-analysis-v4.skill
```

解压技能包到本地目录：

```bash
unzip stock-analysis-v4.skill -d ./unpacked
```

## 备注

这个仓库更偏向“发布包归档仓库”，保存的是可分发的技能包和示例页面，而不是已经解包后的源码工作区。

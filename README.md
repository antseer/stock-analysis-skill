# Stock Analysis Skill

这个仓库用于保存 `stock-analysis` 技能的发布包，以及一个可直接打开的可视化报告示例。

当前仓库里的核心文件：

- `stock-analysis-v4.skill`：当前技能打包文件，实际是一个 zip archive，内部包含 `SKILL.md`、分析脚本、文档和测试文件
- `stock-dark-report.html`：静态深色版股票分析报告示例，可直接在浏览器里打开预览
- `README.md`：仓库说明
- `.gitignore`：忽略本地系统文件

## Skill 信息

根据包内 `_meta.json`，当前发布包版本标记为 `v6.2.0`，主要能力包括：

- 美股与加密货币分析
- 8 维股票评分
- 7 档评级体系
- 数据完整度提示
- 批量对比与相对排名
- 股息分析
- 自选股与提醒
- 投资组合管理
- Hot Scanner 热点扫描
- Rumor Scanner 早期信号/传闻扫描
- HTML / Markdown / JSON / Text 多格式输出

## 仓库内容说明

`stock-analysis-v4.skill` 包内可看到以下内容：

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

这个仓库目前更偏向“发布包归档仓库”，保存的是可分发的技能包和示例页面，而不是已经解包后的源码工作区。

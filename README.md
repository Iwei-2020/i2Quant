# qis

Quantitative Investment Strategies (`qis`) 是一个用于绩效分析、组合回测、风险分析、
压力测试和报告生成的 Python 工具包。

它专注于基于价格数据和外部传入的组合权重进行策略度量与报告输出。策略信号和权重生成
逻辑由使用方自行实现。

## 安装

```bash
pip install qis
```

本地开发：

```bash
uv sync --group test --locked
uv run --no-sync pytest
```

## 主要模块

- `qis.utils`：pandas、NumPy、日期、采样和通用辅助工具。
- `qis.perfstats`：收益、回撤、波动率、夏普指标、市场状态和归因分析。
- `qis.plots`：可复用的绘图工具和衍生分析图表。
- `qis.models`：Bootstrap、协方差、回归、滚动统计和非平滑处理工具。
- `qis.portfolio`：组合数据模型、回测、风险分析、压力测试和报告。
- `qis.market_data`：外汇、因子和市场数据容器。

## 示例

可运行示例位于 `examples/`。

常用入口：

- `examples/getting_started/`
- `examples/perfstats/`
- `examples/portfolios/`
- `examples/factsheets/`
- `examples/market_data/`
- `examples/models/`

## 文档

项目文档位于 `docs/`，包级别说明位于 `src/qis/docs/`。

## 许可证

MIT。详见 `LICENSE.txt`。

## 免责声明

本项目用于研究、分析和报告流程，不构成交易执行系统或投资建议。

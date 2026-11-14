# DSparkX

DSparkX 是对 DeepSeek [DeepSpec](https://github.com/deepseek-ai/DeepSpec) 中 DSpark 投机解码草稿模型的改进：**共享表征 → 通用轮廓专家 → K 小专家并行解码 → 逐位裁决 → 被拒绝候选留作线索、补齐前缀再上**。

## 代码在哪

完整代码（含上游 DeepSpec 全部源码与历史）托管在 fork 仓库：

**https://github.com/lmlmagklm/DeepSpec**

- 设计文档：`docs/dsparkx_design.md`
- 模型实现：`deepspec/modeling/dsparkx/`
- 训练器：`deepspec/trainer/dsparkx_trainer.py`
- 裁决-线索回补闭环评测：`deepspec/eval/dsparkx/`
- 训练配置：`config/dsparkx/dsparkx_qwen3_4b.py`
- 冒烟测试：`tests/test_dsparkx_smoke.py`

本仓库仅作为名称占位与入口说明。

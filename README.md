# Stroke ER

卒中急诊床旁 PWA 原型：NIHSS、mRS、GCS、ASPECTS、卒中时间轴与病程记录生成。

> 临床辅助工具，不替代正式 NIHSS 培训、影像判读、医院卒中流程或医嘱系统。请勿在公开演示版中保存真实患者身份信息。

## 卒中单元评估（增量模块）

- Barthel 指数（BI，10 项，0–100 分）：填写全部条目后显示总分。来源：Mahoney FI, Barthel DW. *Maryland State Med J*. 1965;14:56–61。原量表版权归 Maryland State Medical Society，非商业使用须保留引文；修改或商业使用需取得许可。
- GUSS 吞咽筛查（0–20 分）：依开发者公布的[简体中文版及培训资料](https://www.dysphagie-trapl.at/toolbox/guss-translations/)逐阶段操作，任何阶段未满 5 分即停止后续试吞。仅供受训医护人员床旁使用；公开网页使用量表内容的授权范围仍待权利方书面确认。
- NRS 2002：初筛四问，任一“是”进入终筛（营养状态 0–3、疾病严重程度 0–3、70 岁及以上加 1）；≥3 分提示营养风险。依据 [ESPEN 原始表](https://www.espen.org/documents/Screening.pdf)。
- 营养支持记录：记录是否需要支持、实际启动情况、启动时间、途径和备注，汇入病程记录。筛查结果不自动等于营养支持医嘱。

新模块结果保存在本机 `localStorage` 的 `strokeERAssessV1`；请勿在任何自由文本中填写患者身份信息。原有 NIHSS、mRS、GCS、ASPECTS、时间轴、病程及 IVT 核对入口保留。

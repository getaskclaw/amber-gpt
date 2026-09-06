# amber-gpt

用私有题库 **AMBER** 每周实测 GPT 系模型(含不同推理档位),只公开结果,不公开题目。
English: [README.en.md](README.en.md)

## 这是什么

- 每周一期 `results/YYYY-Www.md`：同题、同 harness，对目标模型跑全库；同模型不同 effort 档位并排。
- 一期固定报告：题集规模与哈希、每案 d2 分与通过/失败、终端终态、token 用量与时延、环境指纹、按证据纪律写的定性裁决。
- 题目、oracle、transcript、中间产物**永不公开**(见下「发布纪律」)。
- 姐妹仓:[amber-crof](https://github.com/getaskclaw/amber-crof)(CrofAI 周测)、[amber-ollama](https://github.com/getaskclaw/amber-ollama)(Ollama Cloud 周测)。

## 发布纪律(红线)

1. 只发：分数与聚合、token 用量、速度、定性裁决。
2. 永不发：题目内容、oracle/判分器、transcript、考生工作区、任何能复原题面的中间产物。
3. 每期必钉：模型 ID、effort 档、日期(UTC)、harness 版本、每案内容哈希(bundle_sha)。哈希用于对照 [amber-eval](https://github.com/getaskclaw/amber-eval) 的公开哈希清单,自证题集未变。
4. 案号与题目结构属私有面：公开结果里案例只用稳定别名(A-xxxxxxxx,哈希派生)+ bundle 哈希作句柄；内部案号、变体名、题目描述永不出现。
5. 基调：这是社区周测,不是对厂商的攻击。数据说话,措辞克制。

## 一个方法论前提

同名模型、同 provider,两次跑也可能不同分——推理参数、负载、服务端版本都在漂。所以这里的一切结论都带日期与档位,且按周重测。单日数字是快照,不是定律。

## 结果索引

| 期 | 内容 | 结论 |
|---|---|---|
| (首期制作中) | — | — |

## 免责

与 OpenAI 无任何隶属/赞助关系。分数是特定周、特定档位的快照,不构成采购建议。

# 繁體中文用語表

本譯本的用語鎖。後續章節沿用此表，不另起譯名。

登記：繁體中文技術寫作。機器學習社群已有固定譯名的，用固定譯名；產品、論文題名、API、程式識別字保留英文。

兩條必須分開的詞：

| English | 中文 | 不用 |
|---|---|---|
| inference | 推論 | 推理 |
| reasoning | 推理 | 推論 |

推論是模型跑前向、產生下一個詞元。推理是鏈條式的思考，例如 chain-of-thought、RLVR。

## 書名與結構

| English | 中文 |
|---|---|
| The LLM Stack | LLM 技術棧 |
| large language model | 大型語言模型（LLM） |
| part | 部 |
| chapter | 章 |
| appendix | 附錄 |
| from scratch | 從零實作 |
| field guide | 實務指南 |
| silicon | 矽晶 |
| agent | 代理 |
| agentic harness | 代理駕馭層（harness） |
| harness engineering | 駕馭層工程 |

## 模型與訓練

| English | 中文 |
|---|---|
| token | 詞元（token） |
| tokenization | 分詞 |
| embedding | 嵌入 |
| attention | 注意力 |
| transformer | Transformer |
| neural network | 神經網絡 |
| pretraining | 預訓練 |
| post-training | 後訓練 |
| mid-training | 中期訓練 |
| fine-tuning | 微調 |
| instruction tuning | 指令調校 |
| supervised fine-tuning (SFT) | 監督式微調 |
| alignment | 對齊 |
| loss | 損失 |
| cross-entropy | 交叉熵 |
| gradient | 梯度 |
| backpropagation | 反向傳播 |
| optimizer | 優化器 |
| learning rate | 學習率 |
| warmup | 預熱 |
| hyperparameter | 超參數 |
| batch | 批次 |
| checkpoint | 檢查點 |
| scaling law | 縮放定律 |
| data | 數據 |
| dataset | 資料集 |
| database | 資料庫 |
| synthetic data | 合成數據 |
| deduplication | 去重 |
| curriculum | 課程式訓練 |
| distillation | 蒸餾 |
| quantization | 量化 |
| mixed precision | 混合精度 |
| parameter | 參數 |

## 平行、記憶體與效能

| English | 中文 |
|---|---|
| parallel | 平行 |
| distributed | 分散式 |
| data parallelism | 數據平行 |
| tensor parallelism | 張量平行 |
| pipeline parallelism | 管線平行 |
| sequence parallelism | 序列平行 |
| expert parallelism | 專家平行 |
| memory | 記憶體（硬體） |
| memorization | 記憶化（模型背下訓練數據） |
| bandwidth | 頻寬 |
| memory-bandwidth-bound | 受記憶體頻寬限制 |
| cache | 快取 |
| KV cache | KV 快取 |
| throughput | 吞吐量 |
| latency | 延遲 |
| kernel | kernel（GPU 上的核心程式） |
| performance | 效能 |
| offloading | 卸載 |
| checkpointing (activation) | 激活檢查點 |

## 推論與服務

| English | 中文 |
|---|---|
| serving | 推論服務 |
| prefill | 預填 |
| decode | 解碼 |
| speculative decoding | 推測解碼 |
| continuous batching | 連續批次 |
| sampling | 取樣 |
| latency | 延遲 |
| prefix caching | 前綴快取 |
| disaggregated | 解耦的 |
| colocated | 共置的 |
| chunked prefill | 分塊預填 |

## 對齊與強化學習

| English | 中文 |
|---|---|
| reward model | 獎勵模型 |
| reward hacking | 獎勵投機 |
| policy | 策略 |
| policy gradient | 策略梯度 |
| rollout | rollout（軌跡取樣） |
| preference | 偏好 |
| verifier | 驗證器 |
| critic | 評論器 |
| advantage | 優勢 |
| replay | 重放 |

## 檢索、代理與評測

| English | 中文 |
|---|---|
| retrieval | 檢索 |
| retrieval-augmented generation | 檢索增強生成（RAG） |
| chunking | 分塊 |
| reranking | 重排序 |
| representation | 表徵 |
| prompt | 提示（prompt） |
| context | 上下文 |
| context window | 上下文視窗 |
| tool use | 工具使用 |
| function calling | 函式呼叫 |
| orchestration | 編排 |
| evaluation | 評測 |
| benchmark | 基準 |
| robustness | 穩健性 |
| confidence interval | 信賴區間 |
| guardrail | 防護欄 |
| red teaming | 紅隊測試 |
| watermark | 浮水印 |
| provenance | 溯源 |
| interpretability | 可解釋性 |
| unlearning | 機器遺忘 |
| differential privacy | 差分隱私 |
| observability | 可觀測性 |
| logging | 日誌 |

## 保留英文的名稱

vLLM、SGLang、FlashAttention、PagedAttention、RadixAttention、LoRA、QLoRA、RoPE、ALiBi、BPE、GRPO、DPO、PPO、RLHF、RLVR、FSDP、ZeRO、Megatron-LM、DeepSpeed、Triton、CUDA、MCP、HBM、GPU、TPU。

## 授權

原著 Prakash Kagitha，*The LLM Stack: From Silicon to Agents*（2026），[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.zh_TW)。譯本須保留作者、原書連結、授權連結，並標明這是翻譯。

- 原書：https://prakashkagitha.github.io/llm-stack-book/
- 原碼：https://github.com/prakashkagitha/llm-stack-book

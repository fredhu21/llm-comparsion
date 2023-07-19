公司	领军人物	模型	基座模型	Transformer架构	参数量	Tokenizer	训练量（Tokens&Flops）	上下文长度	训练语言	位置编码	vocab_size	FlashAttention	MultiQueryAttention	量化支持	训练加速库	开源模式	训练稳定技术	训练并行技术	优化器	主要贡献	HF 下载量
META		LLAMA	LLAMA	Decoder	7B/13B/33B/65B	BPE/SP	"1.4T
2048 A100 * 21Days
~1M A100 GPU Hours"	2K	英语	RoPE	32K	N	N	无官方版本	xformers	对研究开源	"PreLN
RMSNorm
SwiGLU"		Adam W	"1、首个高质量开源自回归语言模型
2、验证Scaling Law：小参数+多样本可以超过大参数"	
META		LLAMA2-Chat	LLAMA2	Decoder	7B/13B/34B/70B	BPE/SP	"2T
1.7M A100 GPU Hours"	4K	英语	RoPE	32K	N	Y	无官方版本		参数开源	"PreLN
RMSNorm
SwiGLU"		Adam W	"1、沿着scaling law的方向再次推进了模型性能
2、官方微调了Chat模型"	
		Open-Llama		Decoder	3B/7B/13B		1T		中英							参数开源		FSDP		受限预算和缺少大规模并行训练的经验，openllama最高只提供13B模型	
Anthropic		Claude2		Decoder												闭源					
OpenAI	Andrej	GPT/GPT2/GPT3	GPT	Decoder	115M/1.7B/175B											闭源				"1、行业里程碑。首个将Scaling Law发挥到极致的千亿模型
2、首个证实大规模参数的DTransfomer架构具备涌现能力。
3、首个提出基于涌现能力实现in-context learning能力的模型"	
OpenAI		GPT4		MOE												闭源					
Google		PaLM																			
Google		Bard																			
Deepmind		Chinchilla		Decoder												闭源					
		Falcon								7B/40B											
		Bloom		Decoder	1B/3B/7B/176B	BPE/SP	"366B
~1M A100 GPU Hours"	2K	多语言	ALiBi	250K	N	N	INT8	"Megatron
DeepSpeed"	"参数开源
训练过程开源"	"BF16
emeddingLN
Deepnorm"	3D并行	Adam	"1、开源了大模型训练过程，对社区有重要借鉴意义
2、过的参数量和行业标杆比过少（一半），导致模型天花板低"	1.6M
Mosaicml		MPT	MPT	Decoder	7B/30B		1T	8K	英语	ALiBi		Y				"参数开源
代码开源"				"1、8K Context Length领先行业
2、训练细节公开
3、系统可分钟级容灾和恢复"	3.43M
百度		文心ERNIE																			
智谱	唐杰	ChatGLM	GLM	Decoder	6B/130B		1T	2K	中英	ROPE		N	N	INT4		参数开源	"DeepNrom
PostLN
EGS"	3D并行	Adam W		1M
智谱		ChatGLM2		Decoder	6B		1T	8K	中英			Y	Y			参数开源		3D并行			1.33M
百川智能	王小川	百川Chat	百川BaiChuan		7B/13B		1.4T	4K		"ROPE
ALiBi"	64K			INT4/INT8		参数开源					1M
面壁智能	刘知远	CPM-Bee		Decoder	1B/2B/5B/10B		1T+	未公开	中英							参数开源					139

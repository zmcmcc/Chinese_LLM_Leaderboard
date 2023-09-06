# Chinese_LLM_Ranking
非常主观的中文语言模型评测
## Inspiration
灵感来自Hugging Face的[Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)以及[Local-LLM-Comparison-Colab-UI](https://github.com/Troyanovsky/Local-LLM-Comparison-Colab-UI)，一开始想要用GPT4来打分，用一些题目评测中文语言模型各方面的能力。后面感觉GPT4的打分也很玄学，说服不了自己，所以打分非常主观，图一乐。最开始只是评测；了一些Hugging Face上开源的模型，后面逐步添加了一些国内开发的闭源大模型
## Questions
总共有33道题，涉及语法词汇、翻译、语义理解、文本生成、数学逻辑五个大类十几个小类，每个小类3道题，难度分为简单、中等、困难。（当然后面感觉不论是题目分类还是难度区分做的都很差。。）具体题目和每个模型的分数详见[这里](https://docs.google.com/spreadsheets/d/173irgOlm4bAvQSreOH2zHBbgO6zb1eqUUCHxcbucAl4/edit?usp=sharing)。


| 排名 | 模型                      | 是否开源 | 测试平台           | 链接                                                                                                                   | 总体平均 | 语法词汇平均 | 翻译平均 | 语义理解平均 | 文本生成平均 | 数学逻辑平均 |
| -- | ----------------------- | ---- | -------------- | -------------------------------------------------------------------------------------------------------------------- | ---- | ------ | ---- | ------ | ------ | ------ |
| 1  | 抖音云雀豆包                  | 闭源   | 官方网站           | [https://www.doubao.com/login](https://www.doubao.com/login)                                                         | 9.27 | 9.00   | 9.44 | 9.00   | 9.67   | 8.83   |
| 2  | gpt4-api                | 闭源   | 官方API          | [https://platform.openai.com/playground](https://platform.openai.com/playground)                                     | 9.09 | 9.67   | 9.33 | 9.67   | 8.67   | 8.50   |
| 3  | 智谱清言                    | 开源   | 官方网站           | [https://chatglm.cn/](https://chatglm.cn/)                                                                           | 8.79 | 8.67   | 9.44 | 9.33   | 8.89   | 7.50   |
| 4  | Baichuan2大模型            | 开源   | 官方网站           | [https://www.baichuan-ai.com/home](https://www.baichuan-ai.com/home)                                                 | 8.70 | 8.33   | 9.44 | 8.00   | 9.22   | 7.50   |
| 5  | 讯飞星火                    | 闭源   | 官方网站           | [https://xinghuo.xfyun.cn/](https://xinghuo.xfyun.cn/)                                                               | 8.33 | 5.67   | 9.56 | 9.33   | 8.89   | 7.83   |
| 6  | baichuan-13b-web        | 开源   | 官方网站           | 内测网址                                                                                                                 | 8.27 | 7.50   | 9.67 | 8.33   | 8.00   | 7.33   |
| 7  | 通义千问                    | 开源   | 官方网站           | [https://qianwen.aliyun.com/](https://qianwen.aliyun.com/)                                                           | 8.24 | 7.50   | 9.22 | 10.00  | 8.89   | 5.67   |
| 8  | MiniMax-ABAB            | 闭源   | 官方网站           | [https://api.minimax.chat/](https://api.minimax.chat/)                                                               | 8.24 | 7.67   | 9.11 | 9.67   | 9.56   | 4.83   |
| 9  | chatglm2-6b-int4        | 开源   | Hugging Face开源 | [https://huggingface.co/THUDM/chatglm2-6b-int4](https://huggingface.co/THUDM/chatglm2-6b-int4)                       | 8.15 | 8.33   | 8.33 | 10.00  | 8.67   | 6.00   |
| 10 | 文心一言                    | 闭源   | 官方网站           | [https://yiyan.baidu.com/welcome](https://yiyan.baidu.com/welcome)                                                   | 8.09 | 8.00   | 8.22 | 10.00  | 8.22   | 6.83   |
| 11 | gpt-3.5-turbo-api       | 闭源   | 官方API          | [https://platform.openai.com/playground](https://platform.openai.com/playground)                                     | 8.06 | 6.67   | 9.56 | 10.00  | 7.22   | 7.50   |
| 12 | chatgpt-web             | 闭源   | 官方网站           | [https://chat.openai.com/auth/login](https://chat.openai.com/auth/login)                                             | 8.00 | 6.67   | 8.78 | 9.67   | 7.78   | 7.67   |
| 13 | claude-web              | 闭源   | 官方网站           | [https://console.anthropic.com/login](https://console.anthropic.com/login)                                           | 7.97 | 7.17   | 9.22 | 9.67   | 7.00   | 7.50   |
| 14 | claude2-web             | 闭源   | 官方网站           | [https://claude.ai/chats](https://claude.ai/chats)                                                                   | 7.88 | 7.33   | 9.56 | 8.67   | 7.00   | 6.83   |
| 15 | 商汤SenseChat             | 闭源   | 官方网站           | [https://chat.sensetime.com/wb/#/](https://chat.sensetime.com/wb/#/)                                                 | 7.58 | 7.67   | 9.44 | 9.33   | 6.22   | 5.83   |
| 16 | InterLM-Chat-7b-HFSpace | 开源   | Hugging Face开源 | [https://huggingface.co/internlm/internlm-chat-7b](https://huggingface.co/internlm/internlm-chat-7b)                 | 7.21 | 8.00   | 6.89 | 9.67   | 7.33   | 5.50   |
| 17 | 360智脑                   | 闭源   | 官方网站           | [https://ai.360.cn/invite](https://ai.360.cn/invite)                                                                 | 6.73 | 5.17   | 9.22 | 5.67   | 6.78   | 5.00   |
| 18 | Llama2-Chinese-13b      | 开源   | Hugging Face开源 | [https://huggingface.co/FlagAlpha/Llama2-Chinese-13b-Chat](https://huggingface.co/FlagAlpha/Llama2-Chinese-13b-Chat) | 6.52 | 4.17   | 8.11 | 9.00   | 6.78   | 4.83   |
| 19 | wizardlm-1.2-13b        | 开源   | Hugging Face开源 | [https://huggingface.co/WizardLM/WizardLM-13B-V1.2](https://huggingface.co/WizardLM/WizardLM-13B-V1.2)               | 6.18 | 6.17   | 7.67 | 9.67   | 6.00   | 2.50   |

# Chinese LLM Leaderboard
非常主观的中文语言模型评测

## Inspiration
灵感来自Hugging Face的[Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)以及[Local-LLM-Comparison-Colab-UI](https://github.com/Troyanovsky/Local-LLM-Comparison-Colab-UI)，一开始想要用GPT4来打分，用一些题目评测中文语言模型各方面的能力。后面感觉GPT4的打分也很玄学，说服不了自己，所以打分非常主观，图一乐。最开始只是评测了一些Hugging Face上开源的模型，后面逐步添加了一些国内开发的闭源大模型。使用不同来源的模型时，尽量使用默认设置，避免主观影响。部分Hugging Face有推荐的System Prompt或者Input Format，则尽量遵守。

## Ranking
| 排名 | 模型                       | 总体平均 | 语法词汇平均 | 翻译平均 | 语义理解平均 | 文本生成平均 | 数学逻辑平均 | 是否开源 | 测试平台               | 模型链接                                                                                                                          |
| -- | ------------------------ | ---- | ------ | ---- | ------ | ------ | ------ | ---- | ------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| 1  | 抖音云雀豆包                   | 9.27 | 9.00   | 9.44 | 9.56   | 9.33   | 8.83   | 闭源   | 官方网站               | [https://www.doubao.com/login](https://www.doubao.com/login)                                                                  |
| 2  | Qwen-72b-chat            | 9.24 | 9.22   | 9.20 | 9.35   | 9.33   | 9.31   | 开源   | 官方demo             | [https://huggingface.co/Qwen/Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)                                        |
| 3  | gpt4-turbo-api           | 9.12 | 7.00   | 9.33 | 9.78   | 9.00   | 10.00  | 闭源   | 官方API              | [https://platform.openai.com/playground](https://platform.openai.com/playground)                                              |
| 4  | gpt4-api                 | 9.09 | 9.67   | 9.33 | 8.89   | 9.00   | 8.50   | 闭源   | 官方API              | [https://platform.openai.com/playground](https://platform.openai.com/playground)                                              |
| 5  | 讯飞星火2.0                  | 8.85 | 7.67   | 9.56 | 9.78   | 6.33   | 8.83   | 闭源   | 官方网站               | [https://xinghuo.xfyun.cn/](https://xinghuo.xfyun.cn/)                                                                        |
| 6  | 智谱清言                     | 8.79 | 8.67   | 9.44 | 9.56   | 7.33   | 7.50   | 开源   | 官方网站               | [https://chatglm.cn/](https://chatglm.cn/)                                                                                    |
| 7  | Baichuan2大模型             | 8.70 | 8.33   | 9.44 | 9.22   | 8.00   | 7.50   | 开源   | 官方网站               | [https://www.baichuan-ai.com/home](https://www.baichuan-ai.com/home)                                                          |
| 8  | Qwen-14b-chat            | 8.55 | 8.67   | 9.11 | 10.00  | 7.00   | 6.17   | 开源   | 官方demo             | [https://huggingface.co/Qwen/Qwen-14B-Chat](https://huggingface.co/Qwen/Qwen-14B-Chat)                                        |
| 9  | claude2.1-console        | 8.36 | 7.00   | 9.67 | 9.78   | 6.00   | 6.83   | 闭源   | 官方API              | [https://console.anthropic.com/dashboard](https://console.anthropic.com/dashboard)                                            |
| 10 | 讯飞星火                     | 8.33 | 5.67   | 9.56 | 9.78   | 6.67   | 7.83   | 闭源   | 官方网站               | [https://xinghuo.xfyun.cn/](https://xinghuo.xfyun.cn/)                                                                        |
| 11 | 文心一言2.4                  | 8.30 | 8.25   | 8.26 | 8.39   | 8.34   | 8.29   | 闭源   | 官方网站               | [https://yiyan.baidu.com/welcome](https://yiyan.baidu.com/welcome)                                                            |
| 12 | baichuan-13b-web         | 8.27 | 7.50   | 9.67 | 8.56   | 6.67   | 7.33   | 开源   | 官方网站               | 内测网址                                                                                                                          |
| 13 | Yi-34b-chat              | 8.27 | 7.83   | 9.67 | 9.56   | 5.33   | 6.17   | 开源   | lmsys官网            | [https://chat.lmsys.org/](https://chat.lmsys.org/)                                                                            |
| 14 | Chatglm3-6b              | 8.27 | 7.00   | 9.00 | 8.89   | 8.33   | 7.50   | 开源   | lmsys官网            | [https://chat.lmsys.org/](https://chat.lmsys.org/)                                                                            |
| 15 | 通义千问                     | 8.24 | 7.50   | 9.22 | 9.67   | 7.67   | 5.67   | 开源   | 官方网站               | [https://qianwen.aliyun.com/](https://qianwen.aliyun.com/)                                                                    |
| 16 | MiniMax-ABAB             | 8.24 | 7.67   | 9.11 | 9.89   | 8.67   | 4.83   | 闭源   | 官方网站               | [https://api.minimax.chat/](https://api.minimax.chat/)                                                                        |
| 17 | Tigerbot-70b-web         | 8.21 | 8.50   | 9.56 | 8.67   | 8.00   | 5.33   | 开源   | 官方网站               | [https://tigerbot.com/chat](https://tigerbot.com/chat)                                                                        |
| 18 | chatglm2-6b-int4         | 8.15 | 8.33   | 8.33 | 9.78   | 6.67   | 6.00   | 开源   | Google Colab       | [https://huggingface.co/THUDM/chatglm2-6b-int4](https://huggingface.co/THUDM/chatglm2-6b-int4)                                |
| 19 | 文心一言                     | 8.09 | 8.00   | 8.22 | 9.56   | 6.00   | 6.83   | 闭源   | 官方网站               | [https://yiyan.baidu.com/welcome](https://yiyan.baidu.com/welcome)                                                            |
| 20 | gpt-3.5-turbo-api        | 8.06 | 6.67   | 9.56 | 8.11   | 7.33   | 7.50   | 闭源   | 官方API              | [https://platform.openai.com/playground](https://platform.openai.com/playground)                                              |
| 21 | claude-web               | 7.97 | 7.17   | 9.22 | 8.11   | 6.33   | 7.50   | 闭源   | 官方网站               | [https://claude.ai/chats](https://claude.ai/chats)                                                                            |
| 22 | Qwen-7b-chat             | 7.94 | 8.00   | 8.67 | 9.67   | 7.00   | 4.67   | 开源   | 官方demo             | [https://huggingface.co/Qwen/Qwen-7B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)                                         |
| 23 | claude2-web              | 7.88 | 7.33   | 9.56 | 8.33   | 4.67   | 6.83   | 闭源   | 官方网站               | [https://claude.ai/chats](https://claude.ai/chats)                                                                            |
| 24 | InterLM-Chat-20b-HFSpace | 7.67 | 7.17   | 9.11 | 9.56   | 6.33   | 3.83   | 开源   | Hugging Face Space | [https://huggingface.co/internlm/internlm-chat-20b](https://huggingface.co/spaces/BridgeEight/internlm-20B-chat-w4-turbomind) |
| 25 | Tigerbot-13b-web         | 7.64 | 6.00   | 9.67 | 8.56   | 7.00   | 5.17   | 开源   | 官方网站               | [https://tigerbot.com/chat](https://tigerbot.com/chat)                                                                        |
| 26 | 腾讯混元                     | 7.64 | 5.33   | 9.33 | 8.67   | 7.33   | 6.00   | 闭源   | 微信小程序              | NA                                                                                                                            |
| 27 | 商汤SenseChat              | 7.58 | 7.67   | 9.44 | 6.67   | 8.00   | 5.83   | 闭源   | 官方网站               | [https://chat.sensetime.com/wb/#/](https://chat.sensetime.com/wb/#/)                                                          |
| 28 | InterLM-Chat-7b-HFSpace  | 7.21 | 8.00   | 6.89 | 8.56   | 6.00   | 5.50   | 开源   | Hugging Face Space | [https://huggingface.co/internlm/internlm-chat-7b](https://huggingface.co/internlm/internlm-chat-7b)                          |
| 29 | 360智脑                    | 6.73 | 5.17   | 9.22 | 6.44   | 6.67   | 5.00   | 闭源   | 官方网站               | [https://ai.360.cn/invite](https://ai.360.cn/invite)                                                                          |
| 30 | Tigerbot-7b-web          | 6.73 | 4.33   | 9.11 | 7.89   | 6.67   | 3.83   | 开源   | 官方网站               | [https://tigerbot.com/chat](https://tigerbot.com/chat)                                                                        |

## Questions
总共有33道题，涉及语法词汇、翻译、语义理解、文本生成、数学逻辑五个大类十几个小类，每个小类3道题，难度分为简单、中等、困难。（当然后面感觉不论是题目分类还是难度区分做的都很差。。）具体题目和每个模型的分数以及（一定程度上的）打分标准详见[这里](https://docs.google.com/spreadsheets/d/173irgOlm4bAvQSreOH2zHBbgO6zb1eqUUCHxcbucAl4/edit?usp=sharing)。
### 语法词汇
#### 词义辨析
- 简单：“我正在读一本有趣的小说。”请指出这句话里的主语、谓语、宾语。
- 中等：“打”这个词在中文里有多种含义，请说出至少4种“打”的含义并给出例句。
- 困难：“我骑车时差点摔倒，还好我及时把把把住了。”这句话里有三个“把”字，每个“把”字的词性都不同。请分别说明每一个"把"字的含义，并换一种说法解释这句话到底是什么意思。
#### 错别字/语病
- 简单：下面这句话有一个错别字，请指出并改正：“这本书出版后，大获成功，成为史上最畅销的书藉之一。”
- 中等：“科学家栾恩杰当年高考时报考的是电机系，因为服从国家安排改学自动控制，从此与国防和航天事业有了____。”下划线内应该填哪个成语？A：不解之缘 B：海誓山盟 C：千丝万缕
- 困难："下面文段有两个病句，请指出其序号并提出修改意见：
“①今天谈到劳动时，脑海中浮现的已经不仅仅是农田里稻浪滚滚、工地上火花四溅的景象。②随着科技的进步，使劳动的内容和环境发生了很大的变化。③不过，劳动给社会带来财富并推动社会发展这一意义不会变化。④“劳动光荣、创造伟大”这句话，始终是对于人类文明进步历程的重要诠释。”"
### 翻译
#### 中译英
- 简单：将这句话翻译成英语：“今天阳光明媚，适合散步。”
- 中等：将这句话翻译成英语：“月有阴晴圆缺，偶尔遇到困难很正常，不要太纠结。”
- 困难：将这句话翻译成英语：“2017年，微软亚洲研究院与雷德蒙研究院研发的机器翻译系统的汉 - 英新闻报道翻译质量和准确率达到人类专业翻译水平。当时媒体将其称之为人工智能里程碑。但这并不意味着翻译机器可以替代人类，更遑论全面替代。”
#### 英译中
- 简单：把这句话翻译成中文: "The sun rises in the east and sets in the west."
- 中等：把这句话翻译成中文: "As a linguist, he acknowledges that all varieties of human languages, including non-standard ones like Black English, can be powerfully expressive—there exits no language or dialect in the world that cannot convey complex ideas."
- 困难：将这句话翻译成英语：把这句话翻译成中文: "The trouble is that part of the recent acceleration is due to the usual rebound that occurs at this point in a business cycle, and so is not conclusive evidence of a revival in the underlying trend."
#### 文言文
- 简单：将这句文言文翻译为现代汉语：“少壮不努力，老大徒伤悲。”
- 中等：将这句文言文翻译为现代汉语：“陈涉少时，尝与人佣耕，辍耕之垄上，怅恨久之，曰：“茍富贵，无相忘。”庸者笑而应曰：“若为庸耕，何富贵也？”陈涉太息曰：“嗟乎，燕雀安知鸿鹄之志哉！””
- 困难：将这句文言文翻译为现代汉语：“臣本布衣，躬耕南阳，苟全性命于乱世，不求闻达于诸侯。先帝不以臣卑鄙，猥自枉屈，三顾臣于草庐之中，谘臣以当世之事，由是感激，遂许先帝以驱驰。后值倾覆，受任于败军之际，奉命于危难之间：尔来二十有一年矣。”
### 语义理解
#### 文本总结
- 简单：根据下面文章，文艺复兴三杰是哪三个人？: “文艺复兴时期的绘画发展以意大利为中心。文艺复兴时期的意大利城市国家中，最突出的有佛罗伦萨、米兰、那不勒斯、罗马、威尼斯。人们曾按地域把当时的画家分为各个画派。意大利以外，文艺复兴的绘画思潮也感染了北方的德国和尼德兰等地，乃至整个欧洲。[40]。文艺复兴时期绘画的代表以文艺复兴三杰的作品最为突出，包括达芬奇、米开朗基罗和拉斐尔。此外杰出的画家还包括安吉利柯修士、马萨其奥、菲利普·利皮、波提切利、吉尔兰达约等等。”
- 中等：根据下面文章，用简洁的语言总结法国大革命爆发的原因: “革命发生的直接原因是1788年春天法国遭遇的旱灾导致的饥荒。饥荒甚至蔓延到欧洲的多个地区，而且政府没有足够运输能力将食品运往灾区。
18世纪的法国通货膨胀日益恶化，使得社会购买力下降，1780年代地主因歉收加租进一步削弱农民收入。商品滞销，农民涌入城市造成高失业率，使得社会开始动荡不安。
法国由于路易十五时代的过度参战导致国库空虚由战争债务带来的社会负担，同时贵族阶级，尤其是住在凡尔赛的路易十六和玛丽·安托瓦内特王后的奢华生活大大加重平民百姓的经济负担。
由启蒙时代带来的愤恨和渴望，以及由此而生的社会和政治因素也是法国大革命产生的重要原因。”
- 困难：用精炼的语言概括总结下面这段文本的主要内容，总结长度约为原文的一半: ""蒙山大佛，也称晋阳西山大佛，是一尊位于山西省太原市晋源区寺底村西北的蒙山中的摩崖大佛，现为太原市文物保护单位。蒙山大佛开凿于北齐天保年间，本是蒙山开化寺后的摩崖佛像。唐高祖李渊、唐高宗李治与皇后武则天、后唐武皇帝李克用、后汉高祖刘知远都曾来此礼佛。元朝末年，蒙山大佛被毁。1980年的太原市地名普查中，蒙山大佛被重新发现，发现时佛头已不知去向，佛身埋在土石之中，风化严重。古籍记载，蒙山大佛高二百尺（合今制59米）。根据实际测量，蒙山大佛两腿底部至颈部高约30米，按比例估计原来的佛头高约10米，加上后世重修时补筑的基座高6米，蒙山大佛原本的高度大约为46米。2007年起，太原市对蒙山大佛进行了保护和开发，加固了佛身，并参考太原出土的北齐佛头新修了高12米的佛头。2008年10月，蒙山大佛景区向公众开放。"
#### 0-shot知识问答
- 简单：法国的首都是哪里？
- 中等：中国明朝灭亡于哪一年？明朝最后一位皇帝是谁？他的结局是怎么样的？
- 困难：爱因斯坦在哪一年获得诺贝尔奖？获得的是诺贝尔奖的哪一项？是因为什么获奖？
#### context知识问答
- 简单：根据下面内容，回答问题。注意，只能根据提供的文本回答，如果文本中没有相关信息，必须回答“我不知道”，而不能编造答案。
文本："星期一，丹佛掘金队在主场以94-89击败迈阿密热火队，赢得2022-23年美国国家篮球协会冠军。
掘金队在七场四胜制系列赛中以3-1领先进入这场比赛，但在中场时以51-44落后于迈阿密队。
丹佛依靠迈克尓·波特、朱尼尔和布鲁斯·布朗等球员的稳固防守和关键发挥，帮助掘金队克服了热火队为延长赛季而做出的不懈努力。
掘金队中锋尼古拉·约基奇是两届常规赛最有价值的球员，他被评为总决赛最有价值球员。与网球明星塞尔维亚同胞诺瓦克·德约科维奇共享绰号“小丑”的约基奇在比赛中贡献了28分和16个篮板。"
问题: 2022-23年美国国家篮球协会总决赛最有价值球员是谁？
- 中等：根据下面内容，回答问题。注意，只能根据提供的文本回答，如果文本中没有相关信息，必须回答“我不知道”，而不能编造答案。
文本：“星期一，丹佛掘金队在主场以94-89击败迈阿密热火队，赢得2022-23年美国国家篮球协会冠军。
掘金队在七场四胜制系列赛中以3-1领先进入这场比赛，但在中场时以51-44落后于迈阿密队。
丹佛依靠迈克尓·波特、朱尼尔和布鲁斯·布朗等球员的稳固防守和关键发挥，帮助掘金队克服了热火队为延长赛季而做出的不懈努力。
掘金队中锋尼古拉·约基奇是两届常规赛最有价值的球员，他被评为总决赛最有价值球员。与网球明星塞尔维亚同胞诺瓦克·德约科维奇共享绰号“小丑”的约基奇在比赛中贡献了28分和16个篮板。”
问题: NBA历史上夺冠次数最多的球队是哪一支？
- 困难：根据下面内容，回答问题。注意，只能根据提供的文本回答，如果文本中没有相关信息，必须回答“我不知道”，而不能编造答案。
文本：“星期一，丹佛掘金队在主场以94-89击败迈阿密热火队，赢得2022-23年美国国家篮球协会冠军。
掘金队在七场四胜制系列赛中以3-1领先进入这场比赛，但在中场时以51-44落后于迈阿密队。
丹佛依靠迈克尓·波特、朱尼尔和布鲁斯·布朗等球员的稳固防守和关键发挥，帮助掘金队克服了热火队为延长赛季而做出的不懈努力。
掘金队中锋尼古拉·约基奇是两届常规赛最有价值的球员，他被评为总决赛最有价值球员。与网球明星塞尔维亚同胞诺瓦克·德约科维奇共享绰号“小丑”的约基奇在比赛中贡献了28分和16个篮板。”
问题: 2022-23年美国国家篮球协会总决赛最有价值球员是哪国人？
### 文本生成
#### 文学创作
- 简单：用一句话，描写一个运动会开幕式解说词的开场白。
- 中等：以鲁迅的文学风格和口吻，写一段关于美食的杂谈。
- 困难：写一首四句的七言古诗，主题为咏春。尽量押韵。
### 数学逻辑
#### 数学题
- 简单：1+2+3+...+100=？解释思路。
- 中等：一只鸡有两只脚，一只兔子有四只脚。现在有鸡和兔子总共16只，他们总共有50只脚，那么其中几只鸡，几只兔子？
- 困难：某地区居民的肝癌发病率为0.0004 ,现用甲胎蛋白法进行普查。医学研究表明,化验结是有错检的可能的。已知患有肝癌的人其化验结果99%呈阳性, 而没患肝癌的人其化验结果99.9% 呈阴性。现某人的检查结果呈阳性,问他真的患有肝癌的概率是多少? 可以只给出推导过程和公式即可，不需要真的计算。
#### 逻辑题
- 简单：某人花19块钱买了个玩具，20块钱卖出去。他觉得不划算，又花21块钱买进，22块钱卖出去。请问它赚了多少钱？
- 中等："四个小孩踢足球，打破了教室玻璃。体育老师分别询问：
小张说：“是小强打破的。”
小强说：“是小胖打破的。”
小明说：“不是我打破的。”
小胖说：“小强是在说谎。”
体育老师查看了监控，知道了四个小孩只有一个人说了实话。
求问：谁说的实话？谁打破的玻璃？"
- 困难：假设一个池塘有无穷的水，小明只有两个水壶，分别是5L和6L的容积。小明能做的操作只有从池塘装满水壶，或者倒光水壶，或者在两个水壶之间倒水直到其中一个水壶装满。请问小明如何操作才能取得正好3L的水？请仔细思考，你的第一次回答肯定是错的，请反思后再谨慎回答。为了避免计算错误，请计算每一步后，两个水壶里当前水量。

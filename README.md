### [chaii: Hindi and Tamil Question Answering](https://www.kaggle.com/c/jane-street-market-prediction/overview) ###
2021 Kaggle Research Code Competition: chaii - Hindi and Tamil Question Answering(Final ***Rank 62/943*** teams)

![image](https://user-images.githubusercontent.com/57436423/143178873-1db03731-1768-4949-83a9-235e93c57574.png)

### Solution: XLMRoberta + weighted layer pooling ###
- 比赛类型：自然语言处理、文本问答任务
- 竞赛任务：预测有关Wikipedia文章的真实问题的答案。提供了带有问答配对的数据集（印地语与泰米尔语）。
- 模型：XLMRoberta 5折单模 + weighted layer pooling
- 评价指标：Jaccard score

通过开源数据进行数据扩增，使用加入weighted layer pooling的XLM-Roberta模型进行Finetune，采用5折交叉验证的方式，各折权重根据CV得分进行分配，最终SOLO取得铜牌。

![image](https://user-images.githubusercontent.com/57436423/143179866-3c26d5a4-32e7-4a06-9b29-32ad6842cd29.png)

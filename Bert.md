# Bert

参考知乎专栏：https://www.zhihu.com/column/c_188941548

#### 背景

从GPT、ELMO及Word2Vec到Bert，bert改造的关键点

![img](dependencies\v2-330788d33e39396db17655e42c7f6afa_r.jpg)

#### 关键改造

- 特征抽取选择Transformer
- 预训练时采用双向语言模型
  - ![](dependencies\v2-146b89cf7ec3eceb349c0d39f8aea228_r.jpg)

- bert集大成体现在哪里？
  - 两阶段模型：第一阶段双向语言模型预训练，这里注意要用双向而不是单向，第二阶段采用具体任务Fine-tuning或者做特征集成
  - 使用transformer抽取特征：transformer抽取特征效果优于CNN与RNN
  - 双向语言模型可以采取CBOW的方法
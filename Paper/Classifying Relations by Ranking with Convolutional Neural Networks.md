### Classifying Relations by Ranking with Convolutional Neural Networks(CR-CNN)
这篇文章在**SemEval-2010 Task 8**的数据集任务基础上，达到了当时的SOTA，F1值为84.1，对比之前的相关工作，没有进行任何的人工特征的提取。
#### 创新点
- 相对比之前的CNN+softmax损失函数，这里定义了Ranking损失函数，通过新的损失函数来训练模型

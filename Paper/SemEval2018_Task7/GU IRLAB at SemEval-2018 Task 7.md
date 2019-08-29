### GU IRLAB at SemEval-2018 Task 7
这篇文章在**SemEval-2018 Task 7**的数据集任务基础上，取得1.1任务第9和1.2任务第5的成绩。
#### 创新点
- 相对比之前的CNN+softmax损失函数，这里定义了Ranking损失函数，通过新的损失函数来训练模型。word embedding + word position embedding 作为特征组合来计算句子表示，然后进一步计算分数，损失函数中使用得到的分数，训练使得loss最小。
- 对于**Other**类别的特殊考虑。没有像之前研究者一样把这个类别与其他9个类别同等对待，因为考虑到这个类别的噪声非常大，因为它由许多不同的不常见类别组成，很难定义它的embedding所以会将噪声带入分类的过程。
- 在取得SOTA的同时，还反向计算出每种类别的最具代表性的三元组，可以作为理解卷积操作的语义编码过程。

#### 相关工作(2010-2014)
![avatar](https://github.com/coderGray1296/Relation-extraction/blob/master/Pictures/1.png)
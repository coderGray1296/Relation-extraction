### GU IRLAB at SemEval-2018 Task 7
这篇文章在**SemEval-2018 Task 7**的数据集任务基础上，取得1.1任务第9和1.2任务第5的成绩。作者使用树结构的递归神经网络。
#### 创新点
- 同时使用句法结构和神经序列模型通过基于树结构的LSTM单元。
- 相比通常的树结构模型，做出了两点改变：不使用实体的表示作为输入，仅仅考虑每个实体的句法head，例如'bag-of-words methods'=>'methods','segment order-sensitive models'=>'models'；其次增加了表示特征，DEP，POS，实体长度，树的深度。
#### 源码
[源码地址](https://github.com/Georgetown-IR-Lab/semeval2018-task7)
### Attention-Based Bidirectional Long Short-Term Memory Networks for Relation Classification
这篇文章在**SemEval-2010 Task 8**的数据集任务基础上，F1值为84，对比之前的相关工作，没有进行任何的人工特征的提取。
#### 创新点
- 相比于之前的方法，不存在人工提取特征的过程，没有使用任何的外部工具提取词法信息和依存关系等高级特征。只使用了word embedding和位置信息。
- 把标签e1,/e1,e2,/e2作为单独的单词作为输入信息输入模型进行训练。
- 使用双向LSTM不仅仅获取past信息还能获取后向的future信息。引入了attention机制来获取更多的语义信息。

#### 相关工作(2010-2014)
![avatar](https://github.com/coderGray1296/Relation-extraction/blob/master/Pictures/2.png)
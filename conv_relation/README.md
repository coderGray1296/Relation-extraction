# conv_relation
## 运行步骤
#### 训练
```
python3 train.py --num_epochs=200 --word_dim=50
```
这里的`num_epochs`参数可以自选，但是`word_dim`由于没有考虑作者对比的300纬度的embedding，所以只考虑50，`/data`中也只有50纬度的预训练embedding
#### 测试
```
python3 train.py --num_epochs=200 --word_dim=50 --test
```
运行之后，`/data`目录中将出现`result.txt`
#### 测试评估计算F1值
```
perl scorer.pl data/test_keys.txt data/results.txt
```
## 论文地址
[Relation Extraction: Perspective from Convolutional Neural Networks](https://github.com/coderGray1296/Relation-extraction/blob/master/Paper/SemEval2010_Task8/Perspective%20from%20Convolutional%20Neural%20Networks.pdf)
## 数据集
SemEval 2010 Task 8 [Full Introduction](https://docs.google.com/document/d/1QO_CnmvNRnYwNWu1-QCAeR5ToQYkXUqFeAJbdEhsq7w/preview)
项目`/data`目录下已经有官方整理好的`train.cln`和`test.cln`可以直接使用
## 运行环境
- Python3
- Tensorflow 1.11+
## 复现结果
根据offical socrer，F1值达到81.34%
![avatar](https://github.com/coderGray1296/Relation-extraction/blob/master/Pictures/3.png)
![avatar](https://github.com/coderGray1296/Relation-extraction/blob/master/Pictures/4.png)
![avatar](https://github.com/coderGray1296/Relation-extraction/blob/master/Pictures/5.png)
![avatar](https://github.com/coderGray1296/Relation-extraction/blob/master/Pictures/6.png)
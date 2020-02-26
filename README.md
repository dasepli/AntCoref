# AntCoref

## 简介

## 数据准备
- 从[CoNLL-2012 Shared Task: Data](http://conll.cemantix.org/2012/data.html)下载训练集/验证集/测试集/scripts等文件，并解压
- 从LDC下载[OntoNotes Release 5.0](https://catalog.ldc.upenn.edu/LDC2013T19)数据集，并解压
- 按照[此教程](https://blog.csdn.net/shuihupo/article/details/79734462)将scripts中的skeleton2conll.py和conll2coreference.py转成python3的形式，也可手动按照[这里](https://github.com/ontonotes/conll-formatted-ontonotes-5.0/issues/2)进行修改


## 实现

## TODO
- 中文指代消解系统
- 中文零指代消解系统
- 中文共指消解系统
- UI
- 事件指代消解系统
- 指代消解标注系统

## 参考
- [Sameer Pradhan](https://cemantix.org/)：OntoNotes构造者
- [End-to-end Neural Coreference Resolution](https://github.com/kentonl/e2e-coref/blob/e2e/setup_training.sh)：数据预处理方式
- [OntoNotes Release 5.0](https://catalog.ldc.upenn.edu/LDC2013T19)

# AntCoref

## 简介

## 数据准备
- 按照[此链接](https://github.com/huggingface/neuralcoref/blob/master/neuralcoref/train/training.md#get-the-data)处理数据
  - LDC的数据可以发邮件加快处理
  - 注意将文件整理到"conll-2012"文件夹里
  - 可以按照[此教程](https://blog.csdn.net/shuihupo/article/details/79734462)自动将scripts中的skeleton2conll.py和conll2coreference.py转成python3的形式，或者使用本repo中提供的scripts
  - 注意skeleton.sh最后一个参数是“conll-2012”
  - 注意Windows系统中的“/\“问题


## 实现

## TODO
- 中文指代消解系统
- 中文零指代消解系统
- 中文共指消解系统
- UI
- 事件指代消解系统
- 指代消解标注系统

## 参考
- [End-to-end Neural Coreference Resolution](https://github.com/kentonl/e2e-coref/blob/e2e/setup_training.sh)：数据预处理方式
- [OntoNotes-5.0-NER](https://github.com/yhcc/OntoNotes-5.0-NER)


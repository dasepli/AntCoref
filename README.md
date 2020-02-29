# AntCoref

## 简介

## 数据准备
- 按照[此链接](https://github.com/huggingface/neuralcoref/blob/master/neuralcoref/train/training.md#get-the-data)处理数据，注意：
  - LDC的数据可以发邮件加快处理
  - 注意将文件整理到"conll-2012"文件夹里
  - 可以按照[此教程](https://blog.csdn.net/shuihupo/article/details/79734462)自动将scripts中的skeleton2conll.py和conll2coreference.py转成python3的形式，或者使用本repo中提供的scripts
  - 注意skeleton.sh最后一个参数是“conll-2012”
  - 注意Windows系统中的“/\“问题
 - 参考[此文档](https://github.com/yhcc/OntoNotes-5.0-NER)对各个中文文件进行整合，构建训练集、验证集、测试集（conll格式）
 - 将conll格式转化为coref格式


## 实现

## 注意事项
- 使用python3, pip3
- 处理了低内存资源文件读入的问题

## TODO
- 中文指代消解系统
- 中文零指代消解系统
- 中文共指消解系统
- UI：[参考](https://github.com/huggingface/neuralcoref)
- 事件指代消解系统
- 指代消解标注系统

## 参考
- [End-to-end Neural Coreference Resolution](https://github.com/kentonl/e2e-coref/blob/e2e/setup_training.sh)：数据预处理方式
- [pytorch-e2e-coref @ YangXuanyue](https://github.com/YangXuanyue/pytorch-e2e-coref)
- [e2e-coref @ kentonl](https://github.com/kentonl/e2e-coref)
- [e2e-coref-old @ tcxdgit](https://github.com/tcxdgit/e2e-coref-old)
- [fastNLP](https://github.com/fastnlp/fastNLP/tree/master/reproduction/coreference_resolution)
- [Pronoun-Coref @ HKUST-KnowComp](https://github.com/HKUST-KnowComp/Pronoun-Coref)
- [coreference-resolution @ shayneobrien](https://github.com/shayneobrien/coreference-resolution)：更整洁的代码


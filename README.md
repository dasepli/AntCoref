# AntCoref

## 简介

## 数据准备
- 下载[OntoNotes Release 5.0](https://catalog.ldc.upenn.edu/LDC2013T19)数据集，可以发邮件给官方加快数据集申请
- 从[Conll-2012 Data](http://conll.cemantix.org/2012/data.html)下载train、test、dev、scripts、scorer等文件并解压，注意根据version将数据集整理到“conll-2012”文件夹里，并将scorer重命名为“scorer”
- 按照[此教程](https://blog.csdn.net/shuihupo/article/details/79734462)将将scripts中的skeleton2conll.py转化为python3格式（也可以直接使用本repo中提供的文件）
- 执行`conll-2012/v3/scripts/skeleton2conll.sh -D path_to_ontonotes_folder/data/ conll-2012`在各个文件中生成conll格式的文件
- 安装[此教程](https://github.com/huggingface/neuralcoref/blob/master/neuralcoref/train/training.md#get-the-data)将训练集、测试集、验证集进行整合
- 执行`python3 minimize.py`将conll文件整理成json文件格式("doc_key"/"sentences"/"speakers"/"constituents"/"constituents"/"clusters")
- 从[此地址](https://pan.baidu.com/s/1tUghuTno5yOvOx4LXA9-wg)（[源地址](https://github.com/Embedding/Chinese-Word-Vectors)）下载预训练的中文词向量，并解压缩
- 执行`python3 get_char_vocab.py`得到中文字表
- 执行`filter_embeddings.py`文件得到过滤版本的词向量集




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
- [AllenNLP coref](https://github.com/allenai/allennlp/blob/master/allennlp/models/coreference_resolution/coref.py#L75)


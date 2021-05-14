# 螺旋桨RNA结构预测竞赛第23名方案

## 环境

Python 3.6

PaddlePaddle 2.0.2

## 训练数据

本项目基于baseline,将网络的最后一层的relu激活函数去掉，并未做出更大的调整。

```
cd work
python src/main.py train --model-path-base model
```
## 预测脚本

```
cd work
python src/main.py test --model-path-base model/best_model_dev\=0.0757
```

## 打包提交文件

```
cd work/output/
zip results.zip *.txt
mv results.zip ~/
```

最后跟目录下的results.zip文件就是用来提交的文件。最终分数3.667。

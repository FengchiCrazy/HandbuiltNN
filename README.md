## 徒手搭建神经网络

参加由格灵深瞳主办的AI Playground的作业。使用C++不能使用任何的开源框架自己搭建深度学习网络训练并输出结果。比赛网站：https://www.hackerrank.com/contests/ai-playground-1/challenges/mnist-1

使用的数据集是Minst，原始图像经过处理后转换成了文本，存放在data文件夹下。内含两个文件:

* `train_2000a.txt`是输入文件，第一行是4个数字，分别是训练样本数n、测试样本数m、图像行数r、图像列数c。从第2行开始是训练样本，一共n行，每行一张图像，最后一列是标签；然后紧跟着测试样本，一共m行，每行一张图像，没有标签。
* `label_2000a.txt`是输出样列，每行一个数字，即0~9，一一对应于输入中的测试样本。
* `example.cpp`是读取这两个文件的样例cpp函数

已经实现的功能有：

* 全连接层
* Sigmoid, ReLU, Tanh
* SoftMaxLoss 

准备实现的功能有：

* 动量收敛策略
* 卷积，池化层

# 李宏毅机器学习 2023 作业

作业文件合集来源于原仓库 [Fafa-DL/Lhy_Machine_Learning](https://github.com/Fafa-DL/Lhy_Machine_Learning)，数据文件较大没有上传，可于原仓库作者维护的公众号【啥都会一点的研究生】获取

## 作业 1

调个 DNN 预测数据，不算太难，但还是调了蛮久才能过双 boss baseline。模板里的 tensorboard 总是抽风，所以还是自己 DIY 了 matplotlib 来画图，但最后感觉似乎也没啥画图的必要？主要的修改是：

- 引入 Adam 优化器
- 引入 L2 正则化
- 加宽加深网络结构
- 选择皮尔曼相关系数超过 0.8 的变量作为输入
- 玄学调参

## 作业 2

当前只过了 strong baseline，不得不说是真难调。过 boss 需要用 RNN，过几天研究一下。网上是个人都在说 BN 和 Dropout 不能一起用，误导了我许久，但这个作业里一起用效果就是好，大抵这就是炼丹罢。主要的修改是：

- concat 23
- 隐藏层 3*1024
- 引入 BN
- 引入 Dropout，输入层 0.3，隐藏层 0.5

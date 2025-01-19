# 南大软院24研究生课程

## 生活

### 图书馆

* 院图书馆如果发现没开门，看看是不是走到后门了
* 微信公众号“江苏省高校数字图书馆JALIS”可以借其他学校图书馆的书，但只能借一个月且不能续借；也可以用来入校参观
* 南京图书馆：借阅要交100押金（可退），最多借4本。书籍不按编号摆放（估计是因为太多了），而是按时间（年），找起来很难

### 云主机

内网访问 172.19.240.2:5000 能创建一个2C4G的云主机。不能直接访问外网；但可直接访问nju开源镜像。\
一种方式是命令行或网页端登校园网，要注意及时登出。\
另一种方式是用SSH通道：在云主机上开启SSH服务端，本机连上去，用`-R`转发到本机proxy软件上。

## 其他人的资料

* https://github.com/123zyzy4/NJU-Software-Course-Materials
* https://www.zhihu.com/column/c_1729514688390623232
* https://eaglebear2002.github.io/categories/南京大学软件学院研究生课程/
* https://github.com/NJU-SE-15-share-review/professional-class 本
* https://github.com/zhangyikaii/NJUCS-Course-Material CS本

本仓库不会包含别人已有的内容，即不全。

## 数据仓库

我个人觉得老师讲的内容是有价值的，思考逻辑非常严谨；涉及的内容大多我之前没了解过，感觉有启发性。可惜我没好好听，当初要是录音录下来就好了。如果对话题感兴趣，推荐上课听，否则就没了。

期末考试有一定难度。虽然是开卷可以带书，但千万不要打算临时学，一定要提前专门花几天时间学习。\
第一题是概念题，然后 聚类、分类、特征相关、关联 各一道算法题。推荐打印以前的卷子及解答，有的题目只改数字。\
其中朴素贝叶斯分类，老师专门提到要用拉普拉斯修正。\
还要打印熵值表，虽然会发log表，但临时算还是很难算。\
熵值如果算出来大于1，就是算错了。因为原数据1:1时熵值是1，经过分类后要减小。

文字复习笔记：https://blog.csdn.net/weixin_44424668/article/details/103227144

24年考试，最后的聚类用的方法是中心点，但好像又不是PAM，而是简化的。

### 视频

* 入门基础概念，比较友好，可惜不全：https://www.bilibili.com/video/BV1er4y1t7GV
* 讲得慢，适合第一次或不急时看：https://space.bilibili.com/87476569/lists/957185
* FP树：https://www.bilibili.com/video/BV1MtqsYHEZr&p=18

### 书

一般各书有一些特色内容，或者某些算法考试不考，跳过不看即可。

* 数据仓库与数据分析教程 9787040341300：写得比较紧凑，数学原理较少。提到了bitmap。是第一项视频对应的书。但校图书馆和南图都没有第二版(9787040548518)，最近的是南林有
* 数据处理与知识发现 9787111605843：有数据预处理知识，有一些数学原理，有不少图表。数仓概念的内容较少，可看下一本补充
* 数据仓库与数据挖掘 9787302483991：每一章后都有实操MSSQL的例子，但也因此占用了版面，对于算法步骤的解释不够、不友好
* 数据仓库与数据挖掘 原理及应用 9787302378617：感觉内容很多，我没细看。可能更适合深入学习、真的想把数仓用起来

## 统计模型：理论与实践

上课讲的话题比较广泛，有不少AI的内容。可以确定跟同名教材(9787111309895)毫不相关。平常用的ppt是英文的，直到期末才分享出来，难以自学。如果对话题感兴趣，推荐上课听，否则就没了。

期末考试范围（PPT）：聚类、分类、EM算法、Gamma函数、概率分布、传统ML NLP。\
实际考试内容：

* 概念题(5*8)：分类的定义、常见NLP任务、解释EM算法、解释泊松分布参数、如何构建 词项-文档矩阵、训练集验证集测试集
* 计算题(12*5)：kNN第一轮、朴素贝叶斯分类、2-gram和条件概率、BoW向量、用极大似然法估计正态分布参数

概率论方面的知识视频：

* 分布：https://www.bilibili.com/video/BV17j411n7UC
* Gamma函数：https://www.bilibili.com/video/BV1Nt411Q7wr https://www.bilibili.com/video/BV1584y117ac
* EM：https://www.bilibili.com/video/BV1h3411y7pD

## 软件安全

教材：软件安全技术 9787111601005\
书的内容，个人认为，对于未接触过安全的同学来说，是相当好的入门读物。

考试范围：除了 3 9 10 11 以外的十章。教程后面的知识性提问记一遍。\
实际也确实就是考这些东西，一共10题。\
如果不追求高分只想及格，应该很容易，毕竟实验占了一大部分。

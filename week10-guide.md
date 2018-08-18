# Week10 项目4 Part1/3
## 统计学

[TOC]

# 学习地图

![-c](http://pb6cho8f0.bkt.clouddn.com/15343016220547.jpg)

本周是统计学项目的Part1，是项目3的基础内容。导学分为两个部分，目标1、2、3、4是对统计学的讲解（本文件）。目标5是项目的第一部分完成（不用担心，这一部分大都是项目3中做过的）。统计学是本项目的重点，请不要被一堆公式吓一跳，项目中用到的都是基础知识。ps：课程里的内容挺多的 

**！注意，1星和2星的可以只看本导学，先大致理解就可以。3星的和项目第一部分是本周重点！**

## 本周知识点

- 数值数据vs分类数据
- Center 集中趋势测量
- Spread 离散程度测量
- 表达式是什么
- 5数概括法
- 直方图的形状
- 描述统计与推论统计
- 概率
- 二项式
- 条件概率
- 抽样分布
- 中心极限定理
- 大数法则
    
## 学习计划

每周的时间进度如下表，注意周六的时间是大家Classin视频讨论的时间，其他的可以灵活调配，记住目标不要拖过一周为妙，加油！请大家仔细看下前面项目3的学习地图，可以灵活的安排下时间，咬紧项目很重要呦！

| 学习时间 | 学习资源 | 学习重点 |
| --- | --- | --- |
| 周3 | /助教/发布当周导学 | 浏览导学文件内容开始学习 |
| 周4 | /Uda/线上内容 | 学习Uda Classroom内容 |
| 周5 | /助教/1v1预约 | 难点可预约1v1语音指导 |
| 周6 | /助教/视频讲解 20:30-21:30 | 讲解本周导学内容、回答疑难问题 |
| 周7 | /助教/根据视频课程学习 | 完成本周内容内容 |
| 周1 | /小结/本周总结 | 总结、笔记、思考 |
| 周2 | /选学/自主学习修养 | 自主学习（选学部分）或调休 |

# /目标1 选修/ 课程1、2:描述统计学第一、二部分

## *|5 数据类型

明白统计学中的两种数量类型：
- Quantitative Data 数值数据：数值数据采用允许我们执行数学运算（例如计算狗的数量）的数值。可以使用数学运算。数量数据又可以分为以下两类（|8 数据类型（连续与离散））
    - Continuous Data 连续数据：比如说狗的年龄。连续数据可以分为更小的单位，并且仍然存在更小的单位。我们可以以年、月、日、小时、秒为单位测量狗的年龄，但是仍然存在可以与年龄关联的更小单位。
    - Discrete Dat 离散数据：比如说狗的数量，仅采用可数值。
    - 实际中我们几乎让所有数据都成为离散数据，很难看出区别。记住连续值可以是任意值，包括小数。
- Categorical Data 分类数据：分类数据用于标记一个群体或一组项目（例如狗的品种 —— 牧羊犬、拉布拉多、贵宾犬等）。用来标记一个群体或一组条目。分类数据又可以分成以下两类（|7 数据类型（定序与定类））
    - Ordinal（Ordered）分类定序：比如说 Rating 排名
    - Nominal（No Order）分类定类：比如说 Breed 狗的种类
- 课程中举例的是老师对于从眼前走过狗狗的统计，数量（几只）和种类（那种狗狗）：

> 图1:数据数据与分类数据
> 
![-c](http://pb6cho8f0.bkt.clouddn.com/15335984061228.jpg)
>
> 图2:数据数据：为什么狗的年龄是连续值
>
![-c](http://pb6cho8f0.bkt.clouddn.com/15336177405804.jpg)
>
> 图3:分类数据：分类定序和分类定类的区别
>
![-c](http://pb6cho8f0.bkt.clouddn.com/15336171781544.jpg)
>

| /数值/ | 连续：身高、年龄、收入 | 离散：书中的页数、咖啡店出现狗的只数 |
| --- | --- | --- |
| /分类/ | 定序：字母成绩等级、调查评级 | 定类：性别、婚姻状况、早餐食品 |

## *|12 概括统计简介

了解了什么是数值数据（Quantitative Data）后，大家还记得前几个项目中我们经常采用均值作为数据分析的一项内容么？当你听到“集中趋势测量”的时候，就是指的这个均值（你不但已经会了，都用过好多次了，是不是心情一下很好？）。

但是均值又个问题，比如说计算平均收入：当把我和老婆的收入区平均值，就能算出我家每个人的平均收入，这个有点意义。但是如果我在电梯里面遇到马云，那么即使当时在电梯里面的平均收入有马云的一半，对我还是没有任何意义。在这种场景下，我们需要进行“离散程度”的测量了，这是一种测量每个值和平均值差异的方法：

- Measures of Center 集中趋势测量（平均数是一种方法，了解学员的一般情况）
- Measures of Spread 离散程度测量（方差，了解学员之间的差异）

除此之外，我们还要观察下数据的形状Shape（熟悉不？）和异常值Outiers（就是有问题的值）

所以说呢，当我们分析数值时，是从这4个方面下手的：

- Center 集中趋势测量:
    - 方法1 均值Mean：Sum of all values divided by the count of values（平均数）
    - 方法2 中位数Median：It is the middle value of a data set（中间那个数，如果是偶数的画，就是把中间两个的值取平均数）
    - 方法3 众数Mode：The most frequent number in a data set（出现次数最多的数；如果次数都相等，就出现无众数的情况；如果有两都出现最多，那么众数就是多个）
- Spread 离散程度测量
- Shape 数据的形状
- Outliers 异常值

## *|19 表达式是什么

这里来扩展下“表达式”是什么（其实加减乘除就是了，你一只在用）。表达式Notation：Common Math language used to communicate 是用来交流的常用数学语言的。可以非常简单（比如说5+3中的+）也可以很复杂，比如这个梯度上升的例子：https://en.wikipedia.org/wiki/Gradient_boosting

## *|22 变量的大小写规则

大写X代表所有变量，小写x代表单个值x1，x2，xn。

## *|25 求和

概率中的聚合有很多种，比如求和公式：

![-c](http://pb6cho8f0.bkt.clouddn.com/15340555400679.jpg)

Σ 符号用于使用求和进行聚合，但是我们可以选择通过其他方式进行聚合。求和是最常见的聚合方式之一。但是，我们可能需要以其他方式进行聚合。如果我们想将所有的值相乘，我们可以使用求积符号 Π ，希腊字母 π 的大写。我们聚合连续值的方式称为积分（微积分中的一种常用技术），它使用以下符号 ∫ ，就像一个拉长的 s。我们不会在此课的练习中使用积分或乘积，但你将来会见到！

## *|26 均值表达式

x-bar就是在x上吗加个横杠，表示x的均值：

![-c](http://pb6cho8f0.bkt.clouddn.com/15340558754956.jpg)

--- 以下进入课程2 ---

## **|1-12 什么是离散程度测量

Measures of Spread ： How far are points from one another
- 5数概括法：Min、Q1、Q2（mean均值）、Q3、最大值（.describe的输出就是这5个数）
- 极差 Range = Max - Min
- 四分卫差 Interquartile Range (IQR) = Q3 - Q1 (中间50%的数据区间）
- 标准差 Standard Deviation：On average, how much each point varies from the mean of the points（每个观测值与均值之差的平均值）标准差是方差的平方根
- 方差 Variance：Average squared difference of each observation from the mean 
- ![-c](http://pb6cho8f0.bkt.clouddn.com/15340577341982.jpg)
- 几个概念的总结：https://classroom.udacity.com/nanodegrees/nd002-cn-basic-vip/parts/4e7e2f82-e05e-4fbe-b29c-fe3169c6dd77/modules/0596b9e8-4a3a-41c3-a929-6c72c0c93925/lessons/c5b785aa-a0e9-45ac-8c4f-6e192829babe/concepts/5f2d9388-2cdc-46d5-81f8-8293edaafdb4
- 使用标准差的好处是使用原始数据的单位（方差带平方运算，所以单位不同），意义是只用一个值就能体现离散程度。标准差经常用于评估金融风险，帮助确定药物在医学研究中的意义，以及测量预测类计算的结果误差，例如预测明天的降雨量或通勤时间。

## *|13 形状

Shape：How to use histograms to determine shape associated with data（就是从图形形状看出数据的分布情况）
- 直方图的形状
    - Right Skewed（右偏态）
    - Left Skewed（左偏态）
    - Symmetric（对称分布，一种是钟形曲线）

## *|20 21 形状与异常值

Outliers: Data points that fall very far from the rest of the values in our dataset（就是明显超出数据集范围的数据，比如年龄统计中有个人322岁，肯定是有问题。注意课程中的例子，扎克伯格的年薪是真实值，但是个异常值，因为他挣得太多了，平均起来没有任何意义）

![-c](http://pb6cho8f0.bkt.clouddn.com/15341700939237.jpg)

这一节课程中有个超详细的outlier的识别文章：http://d-scholarship.pitt.edu/7948/1/Seo.pdf 简单的说，就是如果发现了Outliers，需要注意以下5点：

1. 注意到它们的存在以及对概括性度量的影响。
2. 如果有拼写错误 —— 删除或改正。
3. 了解它们为什么会存在，以及对我们要回答的关于异常值的问题的影响。
4. 当有异常值时，报告五数概括法的值通常能比均值和标准差等度量更好地体现异常值的存在。
5. 报告时要小心。知道如何提出正确的问题。

## *|27 描述统计与推论统计

统计可以分为两类：
- 描述统计：是用来描述收集的数据（就是对现有的数据分析后给出结论，各路ppt大神和excel大表哥们，常做的就是这种）。
- 推论统计：在于使用我们收集的数据对更大的总体数据得出结论（是对未来做预测）。

统计学中的4个基本术语：
- 总体 Polulation：我们想要研究的整个群体。
- 样本 Sample：总体的子集
- 统计量 Statistic：描述样本的数值摘要
- 参数 Parameter：描述总体的数值摘要

![-c](http://pb6cho8f0.bkt.clouddn.com/15342097125386.jpg)
大家可以看上面这个图Uda调查有多少学员喝咖啡的例子。这个例子中前Sample和Statistic是描述统计的，这个例子的描述统计：从5000反馈中得出，73%的学生喝咖啡。而推论统计是使用这5000个回复的数据，得出所有Uda学员喝咖啡习惯的结论。就是通过总体、参数、统计量，得出对参数的推论。因为在现实世界，很少能得到总体（就是每一个）的数据，所以要想知道参数（总体的实际情况），就要使用样本和统计量进行推论了，所以叫推论统计。

在接下来的 课程3:录取案例分析，中对这两节的内容有个实例。在1到11节介绍的是录取案例背景和比率计算，非常友好。在第12节是在workspace中跑一下代码，得出比例的结论（代码的部分之前都接触过很多了，大家看下，run一下就可以得出结论了，看到自己水平的有木有，原来前3个项目没白受虐待啊！）

这课的一个要点是知道统计学的危险，因为当分组不同时（无意的或者为了达到某个结论），分析结果可能完全不同！举了一个辛普森悖论的例子，除了课程中的内容，可以参考这个资料（挺有意思的，有空可以看下，其实根源在基数不同）：https://baike.baidu.com/item/%E8%BE%9B%E6%99%AE%E6%A3%AE%E6%82%96%E8%AE%BA

# /目标2/ 课程4:概率 \ 课程5:二项式

## ***|课程4:概率

概率入门，要认真看的呦。概率和统计学的关系简单讲就是：统计学是根据数据建立模型，而概率是根据模型去预测数据：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342164353268.jpg)

所以呢，为了能够做好统计工作，我们要先了解下概率，本课的小节看着也不少但都很短，普及了概率基础的3个内容（总结的文字内容见 https://classroom.udacity.com/nanodegrees/nd002-cn-basic-vip/parts/4e7e2f82-e05e-4fbe-b29c-fe3169c6dd77/modules/0596b9e8-4a3a-41c3-a929-6c72c0c93925/lessons/f8e3fdae-6759-4dda-aed2-1f094860e2c9/concepts/b1455b30-e76a-47e5-a633-b67d04ede148）

![-c](http://pb6cho8f0.bkt.clouddn.com/15342172627616.jpg)

## **|课程5:二项式

明白了概率的基本概念后，我们来看二项式（二项分布）。课程中是从头到位贯穿了扔硬币的例子，因为硬币有正反两面，所以投掷n次可能会出现很多种组合，这种组合的概率就是二项分布：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342184019216.jpg)

课程中后来引入了公式，如果跟随课程的话可以看懂，有那么一点点的吓人（公式的一个用处不就是吓人一跳么，所以，要学好去吓别人啊）。总结内容在：https://classroom.udacity.com/nanodegrees/nd002-cn-basic-vip/parts/4e7e2f82-e05e-4fbe-b29c-fe3169c6dd77/modules/0596b9e8-4a3a-41c3-a929-6c72c0c93925/lessons/dbd37b8d-f8e0-4708-a919-4b5cebe5ccaf/concepts/d75ae533-4a65-4b15-a8b6-2694b9cf049e

# /目标3/ 课程6:条件概率 \ 课程7:贝叶斯规则 \ 课程8：Python概率练习

## **|课程6:条件概率

其实很多时候，生活中的概率是更加复杂的，比如课程中的这个早起和晨跑之间的关系。如果是夜猫子型，则早起跑步的概率是0，如果是早起型呢，就会有2%的概率去跑步。这种情况就是条件概率，我们不再观察独立事件，第一次投硬币的结果会影响第二次的结果，如下面图：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342276444682.jpg)

接着就是一个癌症检查的例子，如下面图，做一点解释（不要被吓到，就是多了个|，右边是条件，左边是在这个条件下的概率）：
- P（Cancer）是得癌症的概率，P（>Cancer)是没得癌症的概率，这两个概率只和为1（图最上两行）
- 但是检查结果也可能出错，检查的结果是用Positive表示阳性（就是中招了），Negtive表示阴性（安全）
- 所以呢，如果有癌症，检查出来是阳性的几率很大，而检查出来是阴性的几率很小，而且相加为1（图中间两行）
- 同理，如果没有按整，检查出来是阴性的几率很大，而检查出来是阴性的几率很大，而且相加为1（图最后两行）
- 本节课明白这点就行了，后面例子还将到了全概率公式了解就可以，总结链接：https://classroom.udacity.com/nanodegrees/nd002-cn-basic-vip/parts/4e7e2f82-e05e-4fbe-b29c-fe3169c6dd77/modules/0596b9e8-4a3a-41c3-a929-6c72c0c93925/lessons/7ddcb2e7-82be-4b2c-acc0-3e251914ac23/concepts/dac5629c-7c17-48be-8fed-1796953d1326

![-c](http://pb6cho8f0.bkt.clouddn.com/15342285858749.jpg)

## *|课程7:贝叶斯规则

接下来是到了贝叶斯规则这一课，核心的内容是下面这个图（这部分选学）：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342531934360.jpg)

- 先验概率 * 测试证据 = 后验概率
- P(C,Pos)表示后验概率。其中的C是得癌症的几率，Pos表示化验结果为阳性。
- 课程中举例癌症的例子非常贴切，有时间的可以看下来（如果对概率比较生，看3-5遍，就比较清楚了）
- 这个说明也很不错： http://blog.sina.com.cn/s/blog_87e96ae20101d204.html
- 如果能看懂20节的小节，就说明掌握了（可以放到通过以后再看）
- 20小节之后可以不看，是表深入的在无人车应用的例子（Uda校长出马的地方和无人车抢相关呦）

![-c](http://pb6cho8f0.bkt.clouddn.com/15342552300545.jpg)

## **|课程8:Python概率练习

- 这节其实就是把概率的内容落地到Python代码实现上，把所有内容和实例workspace的代码run一遍能看懂就可以了。
- 这部分在项目中有用到，要求看懂能查。
- 第7节的总结非常全面，推荐仔细看完：https://classroom.udacity.com/nanodegrees/nd002-cn-basic-vip/parts/4e7e2f82-e05e-4fbe-b29c-fe3169c6dd77/modules/0596b9e8-4a3a-41c3-a929-6c72c0c93925/lessons/33860189-96c0-40cf-8f12-5772c8b8c790/concepts/d05061c9-efe7-46bf-a135-011ee6773b6d

# /目标4/ 课程10:抽样分布于中心极限定理

在开始课程11之前（下周的），先简单的介绍下 课程10:抽样分布与中心极限定理，这一章的内容是延续课程2中的内容。首先要记住推论统计学的定义：Inferential Statistics - Drawing Conclusions about a population based on data collected from a sample of individuals from that population. 根据总体中的样本，得出关于总体的结论。

那么既然是通过样本推算出总体，那么如果我们的样本不一样，结果会不会不同呢？当然会不一样，请看课程中下面的图：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342939100863.jpg)

这张图特别的赞，我来解释一下：
- 大家看图中有4个深浅不一的蓝色区域，每个区域的边缘都通过了5个咖啡杯。
- 绿色的是不喝咖啡的，红色的是喝咖啡的
- 所以在这5个杯子中，就可以算出不喝咖啡的比率
- 比如有香蕉那个1个绿杯子，4个红杯子，所以不喝咖啡孩子的比率是1/5=0.2
- 而左下角的就是0.6，以此类推
- 那么，如果我们随机取很多次5个样本的话，每个样本就会有一个比率，抽象成下面的图：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342942296999.jpg)

- 当我们把这些随机样本的比率做统计的话，会发现他们的分布是正态分布的（中间多，两边少，像个倒扣的钟一样～没见过？准你请假去看《邪不压正》里的彭于晏还不行）。
- 这个规律就是中心极限定理：样本容量足够大，平均数的抽样分布越接近正态分布。适用于一下统计量中：

![-c](http://pb6cho8f0.bkt.clouddn.com/15343002988921.jpg)

- 有图有真相：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342944294937.jpg)

代码练习在第18节，有一点要说一下：

```python
# 首先设定一个空list
means_size_3 = []
# 从总体中抽取3个，抽取10000次，把每次的mean存到上面的list里
for i in range(10000):
    mean_size_3 = np.random.choice(pop_data,size = 3).mean()
    means_size_3.append(mean_size_3)
```

接下来是抽样分布的练习，这里请大家run一遍，熟悉随机数的代码运用（项目里要用的到）：

```python
# 导入numpy使用随机函数
import numpy as np
# 设定seed，seed的作用是设定了（n）以后，每次随机都能得到相同的抽样
# 这种情况在还原分析过程时非常有用
# 设定了之后就一直有效，直到被覆盖
np.random.seed(42)
students = np.array([1,0,1,1,1,1,0,0,0,0,1,1,1,1,1,1,1,1,1,1,0])
```

```python
# 注意在jupyter 中，seed的设置要和choice在一个代码框才生效
# 所以再输入一遍
np.random.seed(42)
# 此处是用np.random.choice把学生进行抽样，（）为参数
# 第1个参数是数据，就是students
# 第2个参数是抽样的个数
# 第3个参数replace默认= Ture，就是可以再次选中被取到的数
# True的情况适合用在两个骰子。从1-6取，取到1之后还可以取到1
# 学生这个例子要用False，因为一个学生被取走了，就不可以再取了
# random.choice的官方文档
# https://docs.scipy.org/doc/numpy/reference/generated/numpy.random.choice.html
sample = np.random.choice(students,size = 5 ,replace = True)
sample
```

其实课程中在咖啡的例子里是抽样后再放回去的（就是可以再次选中），这种方法叫自展法（bootstrap），就是取出任一个元素，再次选中它的概率不变。这种方式的意义是在样本不变的情况下能够更好的推论出参数：No more data needed to gain a better understanding of the parameter. 自展法为什么有效的说明：https://stats.stackexchange.com/questions/26088/explaining-to-laypeople-why-bootstrapping-works

接下来的一节对于项目4的所有统计学符号做了统计，参数是总体的指标，统计量是样本的指标，如下图，如果有疑问请参见（https://classroom.udacity.com/nanodegrees/nd002-cn-basic-vip/parts/4e7e2f82-e05e-4fbe-b29c-fe3169c6dd77/modules/0596b9e8-4a3a-41c3-a929-6c72c0c93925/lessons/4757541f-77eb-4df6-9ebf-9485a3383dd3/concepts/6802cfeb-3e8f-4218-b3e7-bbc535ae27f0#）：

![-c](http://pb6cho8f0.bkt.clouddn.com/15342985047808.jpg)

在之后，又出现一个新的定理，大数定理：Law of Large Numbers - The Larger our sample size, the closer our statistic gets to the parameter. 翻译过来有点废话的意思：随着样本容量增加，样本平均数越来越接近总体平均数。 接下来是介绍了3中最常见的估算技巧（知道名字就行，想深入点链接）：

- 最大似然估计 https://en.wikipedia.org/wiki/Maximum_likelihood_estimation
- 矩估计方法 https://onlinecourses.science.psu.edu/stat414/node/193/
- 贝叶斯估计 https://en.wikipedia.org/wiki/Bayes_estimator

后面的代码，先生成了3000个gamma分布的数据，分别取5，20，100样本，看看和参数的差距（非常明显的在缩小，符合大数定理）：

```python
import numpy as np
import matplotlib.pyplot as plt

%matplotlib inline
np.random.seed(42)

# gamma是一种分布（官方有个图比较直观）
# 参考：https://zh.wikipedia.org/zh-hans/%E4%BC%BD%E7%8E%9B%E5%88%86%E5%B8%83
# 官方：https://docs.scipy.org/doc/numpy/reference/generated/numpy.random.gamma.html
pop_data = np.random.gamma(1,100,3000)
plt.hist(pop_data)

# 参数
pop_data.mean()
100.35978700795846

# 取5个样本
np.random.choice(pop_data,size = 5).mean()
179.26530134867892

# 取20个样本
np.random.choice(pop_data,size = 20).mean()
143.10974179021264

# 取100个样本
np.random.choice(pop_data,size = 100).mean()
117.0757073569392
```

# /彩蛋/ 统计学深入资料

各位同学如果对统计学感兴趣，想深入一些的话，强烈推荐Uda高级数据分析助教任锐大大的统计学系列：

https://github.com/mengfanchun2017/DAND-Basic/blob/master/Project4/Statistics-Plus.zip

也一并附上项目4文件打包：
https://github.com/mengfanchun2017/DAND-Basic/blob/master/Project4/p4files.zip








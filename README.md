# Tasks_for_Rookies

欢迎来到[计算机视觉实验室](http://cv.nankai.edu.cn/)新手村。新手任务共分为以下几个部分：

>机器学习与深度学习基础

>文献搜集与特定领域发展情况总结

>深度学习编程框架学习与算法实现

>论文写作与rebuttal

>中英文邮件相关


## 1. 机器学习与深度学习基础

+ [机器学习（西瓜书，周志华著）](https://www.zhihu.com/question/39945249)；

***任务***：细读第二到第十四章，并任选一章整理分析。

+ [深度学习（花书，Goodfellow，Bengio等著）](https://github.com/zsdonghao/deep-learning-book/blob/master/dlbook_cn_public.pdf)；

***任务***：从第五章以后精读（尤其是7、8、9、11、12），理解并归纳机器学习中的正则化方法、优化方法以及卷积等操作。英语基础好的同学最好看英文版，以熟悉相关术语。

+ [斯坦福CS231n CNN for Visual Recognition](https://www.bilibili.com/video/av53754154?from=search&seid=6020411155113851809)，总时长约20小时；

***任务***：完成至少三次课堂作业，同时锻炼英语能力。


## 2. 文献搜集与特定领域发展情况总结

在Idea形成之前，应首先确定一个**大方向**，以下方式二选一：
+ **技术**导向：致力于改进某种通用技术，并在不同任务（或标准数据集任务）上进行验证，如神经网络的改进，zero shot方法改进等；
+ **任务**导向：致力于改进某种特定的问题或任务，如情感分类，皮肤病识别，图像翻译等。

****

确定大方向后，便获得了初始的关键词（如zero shot learning，Image-to-Image Translation等），按以下方式进行进行文献搜集，

+ **顶会顶刊关键词搜索**

   + 近三年顶会论文阅读，包括：[CVPR](http://openaccess.thecvf.com/menu.py)，[ICCV](http://openaccess.thecvf.com/menu.py)，[ECCV](http://openaccess.thecvf.com/menu_other.html)，[ICLR](https://openreview.net/group?id=ICLR.cc)，[NeurIPS](https://openreview.net/group?id=NIPS.cc)，[ICML](https://openreview.net/group?id=ICML.cc)等；（*在较广泛的范围内选题，也可以在大量泛读最新会议论文的基础上审视自己的兴趣以及业界研究热点的所在*）

   + 近五年顶刊论文阅读，包括：[TPAMI](https://ieeexplore.ieee.org/xpl/mostRecentIssue.jsp?punumber=34)，[TIP](https://ieeexplore.ieee.org/xpl/mostRecentIssue.jsp?punumber=83)，[IJCV](https://link.springer.com/journal/11263)等；

   注意事项：培养**对于优秀论文的鉴别能力**，以此来合理分配阅读时间。评价指标包括但不限于：论文出处（会议期刊级别）、类型（oral或poster）、引用量、作者（如Kaiming的文章多数很经典）。

+ **已有论文参考文献交叉搜索**

   + 由目前论文中的参考文献进行交叉搜索，可以找出相关的非近年发表的经典论文，以及题目中无相关关键词的必引论文；

   + 精读经典论文以及最新顶会顶刊工作的Related Work部分，按照作者的综述大量略读该领域文献，找出该领域发展脉络并总结；（**该过程非常重要，相当于构建一个‘论文空间’，每次读到新论文都要对其进行归类，自己工作的Idea也是这个空间中的一个点，也即某个发展方向的延伸或某几个方向的交汇。** 以生成式对抗网络为例，可将现有论文按如下方式大致归类：技术上分为对模型网络结构的设计和对损失函数的设计；任务上分为纯生成任务(强调生成器)和与其他任务如语义分割等的结合(强调对抗思想)；目标上分为解决模式崩溃等训练不稳定性问题、提升生成样本质量和提升其他任务性能等）。

+ **作者及研究组主页搜索**

   + 关注该领域活跃的作者，包括大佬级别和生力军，日常翻阅其主页（获取论文、代码、教程博客及其他动态）；

   + 观察某一研究者所做研究之间的相关关系，为自己的研究思路提供借鉴。

+ **其他搜索方式**

   + 利用[Arxiv](https://arxiv.org/)、[Google Scholor](https://scholar.google.com.sg/)、[dblp](https://dblp.uni-trier.de/)等搜索漏网之鱼。

***任务***：

+ 确定自己的研究大方向，按照以上方法进行文献**搜集**，尽可能全地找到该领域的相关工作，以合理的方式建立索引；

+ 整理文档：概括该领域**发展脉络**（按照领域的各个发展方向分别整理，遵循以下格式：第一篇论文的主要思路，存在问题1和问题2；后一篇论文分析问题1可以有什么解决，怎么解决的；另一篇论文如何解决了问题2；在解决问题1和2的同时又引入了新的问题，后又被如何解决）；

+ 整理**表格**：记录每篇论文题目、出处、作者、单位、代码情况、主要贡献等；

+ 论文阅读：**精读**各领域经典论文（分类领域从AlexNet到DenseNet、目标检测领域从RCNN到YoLo、分割领域从FCN到MaskRCNN、生成领域从GAN到BigGAN等），在最新顶会列表上**大量泛读**（读摘要和Introduction决定是否精读，迅速了解该文章的主要创新点）。

## 3. 深度学习编程框架学习

学习资源：（*最好的学习方式便是安装配置好后自己动手尝试，遇到问题查英文官网上的官方文档，遇到报错查Google解决*）

+ TensorFlow
   + [中文版官方文档](https://www.w3cschool.cn/tensorflow_python/?)

+ PyTorch
   + [中文版官方文档](https://pytorch-cn.readthedocs.io/zh/latest/)

+ MXNet：
   + [动手学深度学习视频课程](https://www.bilibili.com/video/av42355860?from=search&seid=10327628739099351727)，李沐（*分类分割检测等均有实现实例，质量非常高*）
   + [动手学深度学习教科书](http://zh.gluon.ai/)，李沐


***任务***：

+ 学习TensorFlow、Pytorch、MXNet中的至少一个；

+ 安装配置基于Ubuntu + CUDA + CuDNN + Anaconda的深度学习环境，配置相关源以加速相关包的安装，安装相应的深度学习框架并测试；

+ 使用ssh或pycharm、VScode等编译器的远程调试功能，在后台远程连接实验室服务器；

+ 编写代码实现以下任务：

   + 实现CIFAR10数据集分类，使用resnet50框架，体会有/无预训练模型的差异；

   + 实现SD-198皮肤病数据集分类（注意数据读取效率），并以普通Resnet 50分类器为baseline提出三种改进策略，观察结果并分析有效性；

   + 训练Faster Rcnn （任意数据集），并在任意图像上测试；

   + 实现基本的生成式对抗网络，利用celebA数据集生成人脸图像，基于该基准，按照最近提出的方法继续改进。

## 4. 论文写作与rebuttal

+ latex相关：
   + [命令查询](http://www.mohu.org/info/symbols/symbols.htm)

+ **论文结构**

   + **题目**：一篇论文的题目是审稿人及读者首先看到的部分，他们根据题目对文章内容进行猜测、对文章贡献建立预期。题目有较多种风格，如：
      + 缩写+内容，如BING: Binarized Normed Gradients for Objectness Estimation at 300fps
      + 吸引眼球型，如You Only Look Once
      + 中规中矩型，全面表达文章贡献，如Clinical skin lesion diagnosis using representations inspired by dermatologist criteria，题目中包含了：做了什么任务，利用了什么技术，技术的创新点

      题目的选定应注意以下几点：
      + **正确性**：题目中的每个词都应该是被同行轻松接受的（判断的标准：是否曾由老外在顶会顶刊中使用且具有相同表意）
      + **准确性**：是否准确地概括了文章的创新点，关键词是否在文章中多次出现
      + **“美观性”**：用词是否专业，是否吸引眼球

      ***任务***：打开某会议收录论文列表或某大牛论文列表，观察已接收论文的题目，从中学习。

   + **摘要**：大致结构如下：
      + 第1-2句：问题定义及/或重要性，现有方案概述；
      + 第2-3句：现有方案缺点；
      + 第3-5句：本文如何解决/本文技术贡献；
      + 第5-6句：本文取得的效果及本文实验情况。

      写摘要需要千雕万琢，写句子尽量**使用简单句**（单一主谓宾结构，或加入最多一个简单从句）；避免任何的语法标点等错误；逻辑缜密，有前因有后果，不可无中生有，不可自己下结论。
   
   + **Introduction**：大致结构如下：
      + 第一段：问题定义，问题的重要性；
      + 第二段：现有主要方法综述，各自的缺点（需选择对应本文创新点的缺点进行阐述，如本文提高了算法效率，则应重点分析相关工作是如何效率低下的，至于准确率低等本文未改进的缺点可简述或忽略），此为论文的MOTIVATION。
      + 第三段：可能的解决方案（由文章思路决定，可以是分析其他领域应用成功的技术模块对本文任务的适用性，也可以是分析现有工作出现该问题的内在原因）；
      + 第四段：本文所提出的的技术概述，标志词即为In this paper, we propose to ...；
      + 第五段（可选）：本文方法得到的理论保证或实验效果；
      + 第六段：本文贡献总结。

      **注意事项**：
      + Introduction中提到的相关工作的缺陷或本文假设等，均要在方法部分及实验部分有所体现（理论分析、证明或实验验证），即**前后照应**；
      + 每一段的**功能**必须**划分**地非常清楚（一般按照以上5-6段书写），同时段之间要有逻辑连接；
      + 段内的每一句均有足够的**因果或并列**逻辑关系（少数情况下存在让步逻辑等），注意**转折词**如In addition, In specific, Therefore, Sequentially, Actually等的正确使用；
      + 不主动claim贡献，是非问题上不妄下定论，每一个观点均有足够的文献或理论分析作为支撑；
      + 论文的MOTIVATION应足够健壮（选题阶段应说服所有人）；
      + 写作质量的评价指标：从头到尾一口气可读通，不存在任何疑问，即为表意成功。

   + **相关工作**：
      + 分节：要按照本文方法涉及到的技术或解决的任务合理分节，一般包括2-3节；
      + 相关工作的概述要全面客观，重点包括**近年来本文所投稿会议或期刊上接收的（所有的）相关论文**；
      + 避免句式单调，在讲前人工作的做法的同时，分析其相对于本文方法体现出来的缺点，在最后与本文方法做比较。

   + **方法**：

      + 流程图需美观、标准、表意清晰；

      + 介绍方法的实际操作前需讲清楚这样做的动机，讲清楚该操作内在的物理意义，并分析或证明为何该操作可以达到好的效果；
      注意：论文内在地应该满足以下条件：**论文的动机来源正确且具说服力，对相关工作的综述（包括做法和缺陷）合理且全面，提出的方法在理论上可以取得更优的效果，后续实验验证该理论的正确性**；

      + 按照文章类型（理论型或技术应用型）适度添加公式、符号。

      ***任务***：浏览、整理、总结经典论文的流程图，学习其表达方式。

   + **实验**：

      + 至少包含以下几个模块：
         + 实验配置介绍：数据集、评价指标、网络结构、对比方法等；
         + 参数调优；
         + 消融实验：逐个验证本文各个模块的有效性；
         + 相关工作对比：本文方法与目前最好方法进行对比；
      + 最重要的，在报告完结果后应**分析该结果说明了什么现象**（应该是验证了方法部分的某个操作的有效性或Introduction部分某个假设的合理性等，照应前文中的理论分析）

   ***任务***：选定某篇经典论文，分析其论文结构

+ **Rebuttal及Response**

   + 二者区别
   
      + 会议论文Rebuttal有字数或篇幅限制，该阶段不允许对论文进行修改，且所给时间较短（一般1周），需仔细斟酌，最终呈现的是最具有说服力的非常言简意赅的论据；

      + 期刊论文response无字数、篇幅等限制，且所给时间相对较长（大修一般6周），可按照意见对论文进行细致修改，最终提交的是修改好的论文及较长篇的回复。

   + 注意事项

      + 揣摩审稿人语气（根据其评分、用词等），以此决定回复策略；
      + 仔细分析审稿人的concern，以此决定回复的重点。回复时，首先**直接回答**审稿人问题，然后给出**足够的理论、文献支撑**。例如，审稿人讲：虽然本文方法足够有效，但已有的X方法曾提出了类似方法。则回答时的第一句应该是讲本文方法在解决任务、理论支撑、方法定义及实验结果上均不同于（最好在某些方面优于）X方法，然后逐条具体分析；
      + 为每个审稿人的每条意见起一个精确的**小标题**，以此在促进版面易读性的同时体现我们对审稿人问题的理解程度；
      + 回复时（尤其是期刊Response时）应尽量从多个角度进行分析，注意合理地按照逻辑进行分条。

   ***任务***：查看实验室某两篇论文（会议期刊各一篇）的投稿历史，阅读并分析其投稿版本、获得的审稿意见、会议论文的rebuttal或期刊论文的response及修改稿、会议论文最终意见或期刊二审意见、论文最终接收版本。对照以上条目进行分析，体会与审稿人进行文字交流的过程。

## 5. 中英文邮件相关

在研究过程中与导师、合作者等人交流的一个重要渠道便是邮件，以下简述中英文邮件的基本格式和注意事项。

+ **基本格式**

   + 中文：
   尊敬的x老师：
     近期工作的主要进展包括：1）xxx采取了xxx操作，取得了xxx结果，该结果符合预期（为什么），主要原因可能是xxx；2）yyy操作验证不可行，因为xxx；
     接下来的计划是：1）xxx；2）yyy；
     祝好，
     sss

   + 英文：
      + 欧洲合作者（如Paul Rosin老师）：
      Dear Professor, 
      We ... (content)
      Best,
      sss

      + 美国合作者（如Ming-Hsuan Yang）：
      Hi, Ming-Hsuan,
      We ... (content)
      Best,
      sss
      
+ **注意事项**:

   + 邮件应清楚、有逻辑地讲清楚所要讲述的事情。例如，对于**汇报论文工作进展**的邮件，可以包括以下内容：
      + 一句话概括主要进展；
      + 进展1：基于什么样的动机，采取什么样的操作；进行了怎样的实验得到了什么样的实验结果，该结果说明了什么；
      + 进展2类似；
      + 论文目前的版本，相对于上一版本进行了哪些改动；
      + 还有哪些正在进行的写作、实验任务，预期完成时间；
      + 未进行的实验等内容根据截稿时间进行合理安排。

      对于**邀请合作者帮助修改论文**的邮件，应包括以下内容：
      + 礼貌语；
      + 表明来意，讲清楚论文题目、投稿会议期刊名称、截稿日期等基本信息；
      + 询问是否可以帮助修改，并对之前的帮助表示感谢；
      + 详细介绍本文的主要贡献；
      + 介绍你认为的本文需要着重修改的点，以及其他应该提前说明的地方；
      + 再次表示感谢，说明你随时可以回复他的任何问题。
   + 与合作者邮件往来应注意**礼貌**；汇报论文进展应着重对目前结果进行分析，并及时更新计划。
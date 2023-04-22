# micro-arch-learning



## 入门水平
1. 6个月完成一生一芯A线并通过流片考核（附学习记录+git repo）
2. 熟练运用chatgpt解决大多数问题

## 初级水平
1. 能完整看明白超标量处理器设计，独立完成[micro-arch-training](https://github.com/arch-simulator-sig/micro-arch-training) [确定]
2. [论文复现](https://github.com/arch-simulator-sig/gem5-with-chinese-comment)    （2week） [论文复现待定]
3. 独立完成[quard-star-tutorial](https://quard-star-tutorial.readthedocs.io/zh_CN/latest/ch21.html) (4week) [确定，该部分作为高阶软件基础]

## 2023年项目任务
1. 跟着周哥学，学习性能分析工具和方法，熟悉xiangshan的前端架构设计
2. 乱序踩坑，参考志锐的dream-core-v1/v2，参考gem5的实现，看书+论文
3. 实现一个顺序或乱序的开源 simulator + RTL，看大家需求发论文+写项目申报书 [架构未定]
4. 学习和分析时序模型：sparta / gem5 / dreamcore / zsim


## 后续项目任务
1. 在给定的模拟器开发框架下，实现香山模拟器迭代
2. 根据项目需求学习多核、乱序相关知识，完成包括但不限于MIT6.175，MIT6.375，[CS152](https://inst.eecs.berkeley.edu/~cs152/sp21/)，[computer architecture](https://safari.ethz.ch/architecture/doku.php)等相关课程，boom，整理一生一芯S线讲义


我的理解：
1. 先做一个正确的顺序处理器，模块不重要，语言不重要，sky的课作用是让你知道自己写的verilog和自己所想的是否一致，如果自己不能确保，需要刷，做两个，对fpga资源有理解。
 
2. 接着开始乱序踩坑，姚永斌的书只写了单列的模块，没有涉及模块耦合的trick，这里都是比较多的坑，写乱序先保证正确性这就已经非常难了，接着coremark性能调优，积累大量经验，可能会持续很多年，会有挫折，贪生怕死，勿入此门。
 
3. 不存在所谓的正确学习道路，需要踩8年以上的坑才有极小可能成为一名架构师，如果顺序设计占用5%，那么一个正确的乱序占用80%，还有无穷大的空间是用于性能调优，然而要达到黄老师的水平，架构师做到了尽头，还需要后端，模拟等全部精通，天人境界，然而即便这样，经常学到每天只睡5h。

4. chisel：缺乏形式化验证，如果chisel4加上将是绝杀，chisel3加上suggestname勉强能用，但是目前工业界不用，风险太大。

5. 后端：非常多的Magic，一个优秀或者天才的架构师需要能够全局掌控。

6. 模拟器：cpp模型正确的概率远大于rtl，需要对自己模拟器的每一个细节做到完全掌握，虽然k210没有模拟器，但是有黄老师人脑模拟，如果觉得自己更强可以不写。

ref [志锐乱序踩坑之旅](https://docs.qq.com/sheet/DWlh0RXNmWm9PeUdi?tab=BB08J2)

跨时钟域：[文档1](http://www.sunburst-design.com/papers/CummingsSNUG2008Boston_CDC.pdf) [文档2](http://www.sunburst-design.com/papers/CummingsSNUG2001SJ_AsyncClk.pdf)



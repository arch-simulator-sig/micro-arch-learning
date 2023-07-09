# micro-arch-learning



## 进入门槛
1. 6个月完成一生一芯A线并通过流片考核（附学习记录+git repo）
2. 熟练运用chatgpt解决大多数问题

## 今年要做的事情
1. micro arch training 全部看完和做完，包括paper，理解乱序思路，理解采样工具
2. 超标量体系结构入门 -> dreamCore v1+v2（不仅包括代码，还有测试思路，各种仿真工具） ，超标量处理器设计，量化，现代处理器设计，高性能超标量cpu（可选）[熟悉超标量]
3. 完成[quard-star-tutorial](https://quard-star-tutorial.readthedocs.io/zh_CN/latest/index.html) (4week) [确定，高阶软件基础入门]
2. 熟悉E203架构，未来1-1.5内的架构基准，所有模拟器基于该架构进行

## 长期项目任务
1. 超标量体系结构入门
3. 学习和分析模拟器设计方案：sparta / gem5 / dreamcore / zsim / systemc / systemc TLM / o3-beta , 后续有新的再加
3. 针对同一个微架构（蜂鸟E203），编写不同的模拟器设计方案进行评测，探索一种通用的模拟器设计方法
4. 使用探索到的通用设计方法，建模香山，从cycle accurate开始，自底向上进行抽象，逐步过渡到性能调优，性能探索

## 处理器设计示例
1. MIPS R10K
2. Intel P6
3. Alpha 21264
4. PowerPC 620
5. BOOM
6. XiangShan
7. XuanTie


## 后续项目任务
1. 在给定的模拟器开发框架下，实现香山模拟器迭代
2. 根据项目需求学习多核、乱序相关知识，完成包括但不限于普林斯顿体系结构，MIT6.175，MIT6.375，[CS152](https://inst.eecs.berkeley.edu/~cs152/sp21/)，[computer architecture](https://safari.ethz.ch/architecture/doku.php)等相关课程，boom，玄铁，整理一生一芯S线讲义


我的理解：
1. 先做一个正确的顺序处理器，模块不重要，语言不重要，sky的课作用是让你知道自己写的verilog和自己所想的是否一致，如果自己不能确保，需要刷，做两个，对fpga资源有理解。

2. 接着开始乱序踩坑，姚永斌的书只写了单列的模块，没有涉及模块耦合的trick，这里都是比较多的坑，写乱序先保证正确性这就已经非常难了，接着coremark性能调优，积累大量经验，可能会持续很多年，会有挫折，贪生怕死，勿入此门。

3. 不存在所谓的正确学习道路，需要踩8年以上的坑才有极小可能成为一名架构师，如果顺序设计占用5%，那么一个正确的乱序占用80%，还有无穷大的空间是用于性能调优，然而要达到黄老师的水平，架构师做到了尽头，还需要后端，模拟等全部精通，天人境界，然而即便这样，经常学到每天只睡5h。

4. chisel：缺乏形式化验证，如果chisel4加上将是绝杀，chisel3加上suggestname勉强能用，但是目前工业界不用，风险太大。

5. 后端：非常多的Magic，一个优秀或者天才的架构师需要能够全局掌控。

6. 模拟器：cpp模型正确的概率远大于rtl，需要对自己模拟器的每一个细节做到完全掌握，虽然k210没有模拟器，但是有黄老师人脑模拟，如果觉得自己更强可以不写。

ref [志锐乱序踩坑之旅](https://docs.qq.com/sheet/DWlh0RXNmWm9PeUdi?tab=BB08J2)

ref [超标量处理器设计书合集](https://caiyun.139.com/m/i?0g5CM8SfyyHjC)  x4Pa提取

ref [IA&C Lab@Fudan - 知乎 (zhihu.com)](https://www.zhihu.com/column/c_1236963527866175488)

ref [已经做完的micro-arch-learning，禁止参考答案](https://github.com/MaxKev1n/micro-arch-learning)

ref 量化研究方法第六版

跨时钟域：[文档1](http://www.sunburst-design.com/papers/CummingsSNUG2008Boston_CDC.pdf) [文档2](http://www.sunburst-design.com/papers/CummingsSNUG2001SJ_AsyncClk.pdf)


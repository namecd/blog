---
title: 2024秋开源操作系统训练营二阶段总结-namecd
date: 2024-11-18 14:31:29
tags:
    - author:namecd
    - repo:https://github.com/LearningOS/2024a-rcore-namecd
---

## 二阶段 rCore 总结
rcore已经顺利完成，跟着教程走来，收获很多。

上次参加训练营因为时间安排的原因，rcore没有做完，停留在了ch3，一直是个遗憾。在今年下半年腾出时间了，想着弥补以前的遗憾，同时也想着深入地学习一下rcore并练习一下rust语言，于是又开始了新一次的尝试。

总体上来说rcore的感触还是挺深的，全神贯注地投入一件事让人着迷。跟着文档一步一步了解rcore的架构，然后在此基础上进行修改完善。在这个过程中，让我对课堂上学到的操作系统的更进一步深入，对操作系统的结构有了进一步的理解。在ch8写银行家算法的时候，本来觉得这个算法很简单，就像在操作系统课上学到的那样就好。但是实际上实现起来还是有很多细节需要注意。

此外还有文件系统那一章节，文件系统应该是这个项目中最难的部分。但是和一个比较完善的操作系统比较起来，这又是一个最简单的版本。麻雀虽小五脏俱全，通过这个小型文件系统，对linux的文件系统有了更深刻的印象。很多只是在课本上听到过的抽象的概念开始具象化，这就是不断学习深入的意义。

在学习的过程中自然而然地遇到了很多困难，通过反复读文档 + 读源码 + 去网上查资料总会解决，只要敢于大胆修改代码，其实只要行动起来，就没什么困难。在之前的学习中可能对于修改代码畏畏缩缩，怕出错，破坏原有的代码，但是实际上有github和本地的commit，没什么好怕的，大不了回滚到之前的版本，重头再来。

我二阶段晋级应该是比较晚了，在ch8中遇到了一些我解决不了的bug，自己明明反复看代码 + 读文档都没感觉有什么问题，但是就是过不了测试样例。在此特别感谢我的一个朋友，他在看完我的代码之后，分析可能是finish数组的原因。如果按照我的设计，我在我设计的数据结构中少了finished的标识。所以导致死锁检测不出来。最终我重新编写了代码，完成了ch8的任务。

总的来说，通过这次的rcore练习，我渐渐地学到了更多操作系统深入一些的内容，为以后更进一步的学习打下了基础。感谢开源操作系统训练营，感谢老师和助教的辛勤付出，感谢我的朋友的帮助。希望以后能够继续学习操作系统的知识，为开源社区贡献一份力量。

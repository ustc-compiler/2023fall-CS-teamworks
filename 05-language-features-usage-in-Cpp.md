# An Empirical Study of Language features usage in C/C++

**[Repository here. (Private now)](https://github.com/Starrybook/ccscaner)**

## Team members

| Student ID | Name   | Github id                                   |
| ---------- | ------ | ------------------------------------------- |
| PB21061327 | 王志成 | [Starrybook](https://github.com/Starrybook) |
| PB21111656 | 余淼   | [Ymm-cll](https://github.com/Ymm-cll)       |
| PB21111682 | 龚劲铭 | [Gjmustc](https://github.com/Gjmustc)       |

## Abstract

本项目旨在分析目标语言`C/C++`的各项语言特性和机制在开源项目中的使用情况。在实现中将目标特性划分为了$\text{Template \& Modular Programming}$ 、$\text{Concurrency \&Multithreading}$、$\text{Memory Management}$、$\text{Exception Handling}$、$\text{Polymorphism \& Overloading}$、$\text{Reference Control}$、$\text{Function}$、$\text{Type System}$等八个类别，并在每一类别中选取了相应的若干特征项；继而利用我们完成的工具`CCScaner`对一批开源项目仓库进行了统计分析，得到统计结果。本项目将基于这一统计结果进行进一步的分析与讨论，以加深对这一经典语言的诸多特性的理解；并与现有的基于其他高级语言特性的相关研究结论进行对照，从而在新的角度认识不同语言特性在实际应用中的作用。



## Target

1.  整理汇总`我们所关注的C/C++`语言特征，划分成为不同类别，并在每一类别中选取若干具有代表性的特征项

2.  基于我们完成的工具`CCScaner`分析`C/C++`的各项语言特征在开源项目中的使用情况，获得基础数据

3.  对得到的基础数据进行分析与讨论，关注：

    1.  `C/C++`语言中的那些特性具有比较显著的影响，并得到大量应用
    2.  不同领域语言使用者的特性使用倾向

    等等。

4.  与现有的基于其他高级语言特性的相关研究进行对照，进行进一步的讨论



## Preliminary route

1.  明确目标语言
2.  讨论语言特性，选择关注点并进行汇总
3.  建立`CCScaner`的项目框架，选择树分析工具，完成外层数据处理脚本
4.  确定数据处理与存储流程，完成对特性表类`cctable`的搭建
5.  基于特性汇总表完成对`demo/`目录的填充，将特征的定义细化到语言实例
6.  完成`CCScaner`项目核心类`ccscaner`，确定对每一个特性项的处理逻辑
7.  分别对单文件和单目录进行调试测试，据此完善项目的每一个组件
8.  对测试仓库进行处理，得到相应数据，从而对特性表、特性处理方法进行反复的再调整
9.  利用已完善的工具`CCScaner`对大量仓库进行分析汇总
10.  对数据进行处理与人工分析，得到初步结论
11.  与现有的相关研究进行对照，进行深入讨论



## Related works

https://github.com/tree-sitter/py-tree-sitter

https://github.com/S4Plus/PyScan

https://ieeexplore.ieee.org/abstract/document/9425916

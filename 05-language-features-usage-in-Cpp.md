# An Empirical Study of Language features usage in C/C++

**[Repository here. (Public now)](https://github.com/Starrybook/ccscaner)**

**[Report.md here. (under ./doc/)](https://github.com/Starrybook/ccscaner/blob/master/doc/Report.md)**

**[Report.pdf here. (under ./doc/)](https://github.com/Starrybook/ccscaner/blob/master/doc/Report.pdf)**

**[How to use this tool. (under ./doc/)](https://github.com/Starrybook/ccscaner/blob/master/doc/scripts-examples.md)**



## Team members

| Student ID | Name   | Github id                                   |
| ---------- | ------ | ------------------------------------------- |
| PB21061327 | 王志成 | [Starrybook](https://github.com/Starrybook) |
| PB21111656 | 余淼   | [Ymm-cll](https://github.com/Ymm-cll)       |
| PB21111682 | 龚劲铭 | [Gjmustc](https://github.com/Gjmustc)       |



## Abstract

本项目旨在分析目标语言`C/C++`的各项语言特性和机制在开源项目中的使用情况。在实现中将目标特性划分为了  Template & Modular Programming 、Concurrency & Multithreading、Memory Management、Exception Handling、Polymorphism & Overloading、Reference Control、Function、Type System  等八个类别，并在每一类别中选取了相应的若干特征项；继而利用我们完成的工具 CCScaner 对一批开源项目仓库进行了统计分析，得到统计结果。本项目将基于这一统计结果进行进一步的分析与讨论，以加深对这一经典语言的诸多特性的理解。



## Target

1.  整理汇总`我们所关注的C/C++`语言特征，划分成为不同类别，并在每一类别中选取若干具有代表性的特征项

2.  基于我们完成的工具`CCScaner`分析`C/C++`的各项语言特征在开源项目中的使用情况，获得基础数据

3.  对得到的基础数据进行分析与讨论，关注：

    1.  `C/C++`语言中的哪些特性具有比较显著的影响，并得到大量应用
    2.  不同领域语言使用者的特性使用倾向

    等等。



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
10.  对数据进行处理与人工分析，得到结论



## Related works

[An Empirical Study for Common Language Features Used in Python Projects](https://ieeexplore.ieee.org/abstract/document/9425916)

[An Empirical Study of Type-Related Defects in Python Projects](https://ieeexplore.ieee.org/document/9436020)

[An Empirical Study of C++ Programs](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=60944615a1a9e432d1d4338b528e60e7dc9de3c3)

[An Empirical Study of Function Overloading in C++](https://ieeexplore.ieee.org/document/4637538)

[Github repository: PyScan](https://github.com/S4Plus/PyScan)

[Tree-sitter official documentation](https://github.com/tree-sitter/py-tree-sitter)

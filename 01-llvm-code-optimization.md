## 基于LLVM的SysYF进阶优化

徐航宇 李牧龙

### 仓库地址

https://github.com/liml0324/SysYF_optimize

### 摘要

本课程项目旨在基于LLVM，结合课堂所学的知识，并查阅学习相关文献及算法，在若干方向对SysYF语言生成的LLVM中间代码进行优化。在有余力的情况下进一步完成汇编代码的生成和优化。

### 相关资源

[支配树算法](https://www.cs.tufts.edu/comp/150FP/archive/keith-cooper/dom14.pdf)

[图着色算法](https://www.sciencedirect.com/science/article/abs/pii/B9781483231877500155)

[基于图着色的寄存器分配](https://www.sciencedirect.com/science/article/abs/pii/0096055181900485)

[基于SSA的寄存器分配](https://pp.ipd.kit.edu/uploads/publikationen/stemmergrabow21masterarbeit.pdf)

### 研究内容

目前可能考虑的优化方法有：

- 1. 消除中间代码中的store，load，alloca指令，指令全部使用寄存器
- 2. 进行活跃变量分析、死代码删除等，避免执行多余的指令
- 3. 采用复写传播、强度削弱、循环表达式外提等更多优化方式进行进一步优化
- 4. 如果进行代码生成和后端优化，则主要考虑寄存器分配问题

### 研究目标

暂定在PW6的SysYF中间代码生成的基础上进行实验。
为方便实现，在PW6的基础上加入去年PW8的代码框架，在其基础上进行修改（大体上将裸指针改为智能指针即可）。

### 组员分工

李牧龙：主要负责LLVM IR的优化

徐航宇：主要负责后端代码部分

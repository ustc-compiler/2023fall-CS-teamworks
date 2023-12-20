## 基于LLVM的后端代码优化

徐航宇 李牧龙

[link](https://github.com/liml0324/2023fall-CS-teamworks)

### 摘要

本课程项目旨在基于LLVM，结合课堂所学的知识，并查阅学习相关文献及算法，在若干方向对后端代码生成进行优化

### 相关资源

[图着色算法](https://www.sciencedirect.com/science/article/abs/pii/B9781483231877500155)

[基于图着色的寄存器分配](https://www.sciencedirect.com/science/article/abs/pii/0096055181900485)

[基于SSA的寄存器分配](https://pp.ipd.kit.edu/uploads/publikationen/stemmergrabow21masterarbeit.pdf)

[支配树的增量计算](https://dl.acm.org/doi/abs/10.1145/202530.202531)

### 研究内容

目前可能考虑的优化方法有：

- 1. 通过支配树完成支配边界的计算，从而完成SSA的构造以及循环不变量提升
- 2. 使用图着色及线性扫描，或其他启发式方法，优化寄存器分配
- 3. 利用找环算法寻找循环，并优化循环中的寄存器分配

### 研究目标

暂定在PW6的SysYF中间代码生成的基础上，采用上述优化方法进行后端代码生成的优化

### 组员分工

徐航宇：主要负责文献调研及算法设计

李牧龙：主要负责算法实现及性能测试
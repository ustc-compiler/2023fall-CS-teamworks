## 图查询语言及其语义分析

### Members
| Name | Student ID | Github ID  |
| ---- | ---------- | ---------- |
| 吴书让  | PB21000179 |[odeinjul](https://github.com/odeinjul)    |
| 罗胤玻  | PB21111627 | [Origami-B](https://github.com/Origami-B) |
| 胡天羽  | PB21111629 | [tyrionhuu](https://github.com/tyrionhuu) |

[2023fall-CS-teamworks](https://github.com/odeinjul/2023fall-CS-teamworks)

### Repo 
[Graph Query Language](https://github.com/odeinjul/gql)

### Report
[Report](https://github.com/odeinjul/gql/blob/main/report.pdf)

### Content

本项目旨在分析图数据处理、查询语言的相关理论和技术实现。通过审视多种常用的图数据处理引擎及其对应图查询语言，该项目将归纳总结各类语言的不足、优势以及特点所在，并且对相关编译流程和优化方式进行探讨，帮助我们更深入地理解图数据语言的发展现状。

### Related Work

[GQL Standard](https://www.gqlstandards.org/)

[openCypher](https://opencypher.org/)

[nGQL](https://docs.nebula-graph.com.cn)

[PGQL](https://pgql-lang.org/)

[AQL](https://docs.arangodb.com/stable/aql/)

[GSQL](https://docs.tigergraph.com/gsql-ref/current/intro/)

[Gremlin](https://tinkerpop.apache.org/gremlin.html)

[openCypherTranspiler](https://github.com/microsoft/openCypherTranspiler/)

[pgql-lang](https://github.com/oracle/pgql-lang/)


### Todo(s)

- 收集图查询语言
- 整理各图查询语言特性，功能实现差异，优缺点
- 选择某几特定图查询语言深入分析语义，以及特有技术（特点）的技术实现原理
- 根据开源项目以及相关文献学习图查询语言的编译流程和优化方式

### Target(s)

- 全面了解业界图查询语言、引擎发展情况以及异同
- 深入语义理解图查询语言的特性以及共同点
- 整理图查询语言的编译流程和优化方式

### Steps

1. 全组共同收集图查询语言，可以从相关综述文献入手，并且补充业界最新项目。因为后期需要深入分析，应以开源项目优先。
2. 审视图数据处理引擎以及图查询语言，选取代表性的若干个作为研究重点。
3. 小组三人各自针对某一图查询语言进行了解，汇总功能实现等方面上的异同。此部分需要定期讨论以同步进度。
4. 在完成对市面上大部分图查询语言的整理之后，选取某几图查询语言进行重点语义理解总结。需要先将此语言的特有功能/特性拆分成多份，以便同步进行分析加快进度。
5. 选取完善的某几个开源编译项目，进行代码探究，整理出图查询语言的编译流程共同点。
6. 选取较为清晰易懂的图查询语言相关优化论文进行探讨，整理出图查询语言的常见优化方式。
7. 整理上述研究所得，形成报告。

### Tips
同时由于下面三点原因，我们选择了纯调研类工作：
    1. 全面理解图查询语言现状需要阅读大量及多种类的文档、文献、代码。
    2. 数据库查询类语言通常只是为了查询，本身较为简单，难以编写复杂代码。
    3. 业界对图查询语言的优化主要关注对最终关系代数的优化，而非对编译的优化（此方面的工作开展需要有关图查询/数据库查询的专业知识，且与编译原理知识关联不大），因此选择只做相关工作的调研.

由于没有代码方面工作，我们主要采用Overleaf直接同步各方面调研工作进展以及记录。

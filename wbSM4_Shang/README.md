白盒SMS4实现
====================================================

本代码基于尚培硕士论文中对肖雅莹白盒SM4的改进二，将肖雅莹白盒SM4中的仿射编码的一部分改为矩阵编码，外部编码均由矩阵实现。


代码需要基于NTL（一个密码学相关的库）的运行环境

wbSM4.cpp wbSM4.h中包含加密所需要的相关方法的声明与实现
先运行generator.cpp文件构造出加密所需的头文件（包含查找表与相应的仿射）
然后运行main.cpp实现加密。
本实现将外部编码与加密部分在同一文件中实现，如果需要可以将外部编码独立出来。

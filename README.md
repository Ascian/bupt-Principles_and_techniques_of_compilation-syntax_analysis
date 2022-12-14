# syntax_analysis
 
## 实验内容

编写语法分析程序，实现对算数表达式的与语法分析。要求所分析算数表达式
由如下文法产生。
* E->E+T|E-T|T
* T->T*F|T/F|F
* F->(E)|num

## 实验要求

在对输入的算数表达式进行分析的过程中，依次输出所采用的的产生式。
* 方法 1：编写递归调用程序实现自顶向下分析。
* 方法 2：编写 LL(1)语法分析程序，要求如下。
    * 编写实现算法 4.2，为给定文法自动构造预测分析表。
    * 编写实现算法 4.1，构造 LL(1)预测分析程序。
* 方法 3：编写 LR(1)语法分析程序实现自底向上分析，要求如下。
    * 构造识别该文法所有活前缀的 DFA。
    * 构造该文法的 LR 分析表。
    * 编写实现算法 4.3，构造 LR 分析程序。
* 方法 4：利用 YACC 自动生成语法分析程序，调用 LEX 自动生成的词法分析程序。

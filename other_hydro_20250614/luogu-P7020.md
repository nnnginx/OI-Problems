## 题目描述


Boolean satisfiability problem (SAT) is known to be a very hard problem in computer science. In this problem you are given a Boolean formula, and you need to find out if the variables of a given formula can be consistently replaced by the values true or false in such a way that the formula evaluates to true. SAT is known to be NP-complete problem. Moreover, it is NP-complete even in case of $3-CNF$ formula $(3-SAT).$ However, for example, SAT problem for $2-CNF$ formulae $(2-SAT)$ is in $P$ .

$#SAT$ is the extension of SAT problem. In this problem you need to check if it is possible, and count the number of ways to assign values to variables. This problem is known to be $#P-complete$ even for $2-CNF$ formulae. We ask you to solve $#1-DNF-SAT,$ which is $#SAT$ problem for $1-DNF$ formulae.

You are given a Boolean formula in $1-DNF$ form. It means that it is a disjunction (logical or) of one or more clauses, each clause is exactly one literal, each literal is either variable or its negation (logical not).

Formally:

$〈formula〉 ::= 〈clause〉 | 〈formula〉 ∨ 〈clause〉$

$〈clause〉 ::= 〈literal〉$

$〈literal〉 ::= 〈variable〉 | ¬ 〈variable〉$

$〈variable〉 ::=$ A . . . $Z |$ a . . . $z$

Your task is to find the number of ways to replace all variables with values true and false (all occurrences of the same variable should be replaced with same value), such that the formula evaluates to true.



## 输入格式


The only line of the input file contains a logical formula in $1-DNF$ form (not longer than $1000$ symbols). Logical operations are represented by $‘|'$ (disjunction) and $‘ \sim ' (negatio_n).$ The variables are $‘A'$ . . . $‘Z'$ and $‘a'$ . . . $‘z'$ (uppercase and lowercase letters are different variables). The formula contains neither spaces nor other characters not mentioned in the grammar.



## 输出格式


Output a single integer -- the answer for $#SAT$ problem for the given formula.



## 题目大意
给定一个由大小写字母（变量），``|`` 和 ``~`` 组成的布尔代数式，求对于给定的变量，有多少种方案使得给定的代数式值为 ``True`` 。

注：

``a|b`` 表示 $a\vee b$ , 也就是 C++ 中的 ``a || b`` 。

``~a`` 表示 $\neg a$，也就是 C++ 中的 ``(!a)`` 。

变量只有可能由单个字母构成。

```input1
a

```

```output1
1

```

```input2
B|~B

```

```output2
2

```

```input3
c|~C

```

```output3
3

```

```input4
i|c|p|c

```

```output4
7

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 




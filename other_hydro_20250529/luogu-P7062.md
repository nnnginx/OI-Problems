## 题目描述
Combinatory logic may be thought as one of computational models allowing to express any computable function as a composition of functions from a small finite basis. In this problem we consider a restricted variant of BCKW basis, BCKI.

Combinator expression in BCKI basis is a string, corresponding to the following grammar:

```plain
⟨Expression⟩ ::= ⟨Expression⟩ ⟨Term⟩ | ⟨Term⟩
⟨Term⟩ ::= ‘(’⟨Expression⟩‘)’ | ‘B’ | ‘C’ | ‘K’ | ‘I’
```

As we can see from the grammar, the expression is a tree of applications where leafs are combinators $B, C, K$ and $I$. The application is left-associative. For example $BIC$ is equivalent to $(BI)C,$ but not to $B(IC)$.

For the sake of the explanation we will use lowercase English letters $(a \cdots z)$ to represent sub-expressions. These lowercase letters will not appear in real data. For example, $BIC$ can be represented by $BxC$ (that is, $B\underbrace { I }_{ x }C)$, $x(\underbrace {BIC}_{ x })$, $xy(\underbrace {BI}_{ x } \underbrace { C }_{ y })$, $Bxy (B\underbrace { I }_{ x }\underbrace { C }_{ y })$, but not by $Bx$.

We say that in expression $pq$ we apply $p$ to $q$. We can employ our intuition by saying that $p$ is a function and $q$ is its parameter. However, the evaluation process is quite different from traditional computation — instead of passing values over fixed expression tree, we evaluate by altering that tree so that the result is also some combinator expression.

To evaluate an expression, we need to select some sub-expression, corresponding to one of the patterns specified in the table below — that is, there should exist such $x$ (and maybe $y$ and $z$) that the pattern from the table becomes equal to the sub-expression. Then we need to replace the sub-expression with the reduction result from the table.

| Pattern | Reduction result |                   Description                   |
| :-----: | :--------------: | :---------------------------------------------: |
| $Bxyz$  |     $x(yz)$      | Composition function (Zusammensetzungsfunktion) |
| $Cxyz$  |     $(xz)y$      |    Exchange function (Vertauschungsfunktion)    |
|  $Kxy$  |       $x$        |      Constant function (Konstanzfunktion)       |
|  $Ix$   |       $x$        |     Identity function (Identitätsfunktion)      |

After the replacement took place we must repeat the process, until there remains no suitable subexpressions. This final expression is normal form of the original one. For example, in expression $CIC(CB)I$ we can make the following letter assignment

$$\underbrace { C }_{ C }\underbrace { I }_{ x }\underbrace { C }_{ y }\underbrace {(CB)}_{ z }I$$

and see that $CIC(CB)I ≡ (((CI)C)(CB))I ≡ (((Cx)y)z)I$ contains $C$ combinator pattern and thus reduces to $((xz)y)I ≡ I(CB)CI:$

$$(\underbrace { C }_{ C }\underbrace { I }_{ x }\underbrace { C }_{ y }\underbrace { (CB) }_{ Z })I \rightarrow (\underbrace { I }_{ x } \underbrace {(CB)}_{ z }\underbrace { C }_{ y })I$$

One more example: $B((CK)I)IC$ expression. Let us first reduce combinator $B:$

$$(\underbrace { B }_{ B }\underbrace { ((CK)I) }_{ x }\underbrace { I }_{ y }\underbrace { C }_{ z } \rightarrow \underbrace { ((CK)I) }_{ x } (\underbrace { I }_{ y }\underbrace { C }_{ z })$$

Now, let's reduce the last $I:$

$$((CK)I)(\underbrace { I }_{ I } \underbrace { C }_{ x }) \rightarrow ((CK)I)C$$

And now we finish evaluation with two more reductions:

$$((\underbrace { C }_{ C }\underbrace { K }_{ x }) \underbrace { I }_{ y }) \underbrace { C }_{ z } \rightarrow (\underbrace { K }_{ K }\underbrace { C }_{ x }) \underbrace { I }_{ y } \rightarrow C$$

It is possible to show that the normal form remains the same irrespectable to the order of evaluation. For example, the following evaluation order:

$$C(K(II)(\underbrace { I }_{ I }\underbrace { C }_{ x })) \rightarrow C(K(\underbrace { I }_{ I }\underbrace {  I}_{ x })(C)) \rightarrow C((\underbrace { K }_{ K }\underbrace { I }_{ x }) \underbrace { C }_{ y }) \rightarrow CI$$

leads to the same result as 

$$C(K(\underbrace {I}_{ I }\underbrace { I }_{ x })(IC)) \rightarrow C((\underbrace { K }_{ K }\underbrace { I }_{ x })\underbrace { (IC)}_{ y }) \rightarrow CI$$

However, as you see, the number of reductions is different: $3$ in the first case and $2$ in the second. This poses an interesting problem -- to find an evaluation order with the minimal number of reductions for a given formula.

Your task is to write a program which finds the minimal number of reductions required for a given combinator expression to be evaluated to its normal form.

## 输入格式


The only line of the input file contains a combinator expression corresponding to the grammar above. The length of the expression does not exceed $30 000$ . The expression contains no whitespaces or symbols not specified in the grammar.



## 输出格式


Output a single integer — the minimal number of reductions required for the given formula to evaluate it to normal form.



## 题目大意
## 题目背景

## 题目描述
组合逻辑可以看作是一种计算模型，允许将任何可计算函数表示为从小的有限基底中选取的函数的组合。在这个问题中，我们考虑 BCKW 基底的一个受限变体，即 BCKI。

BCKI 基底中的组合表达式是一个字符串，对应于以下文法：

```plain
⟨表达式⟩ ::= ⟨表达式⟩ ⟨项⟩ | ⟨项⟩
⟨项⟩ ::= ‘(’⟨表达式⟩‘)’ | ‘B’ | ‘C’ | ‘K’ | ‘I’
```

从文法可以看出，表达式是应用树，叶子是组合子 $B, C, K$ 和 $I$。应用是左结合的。例如，$BIC$ 等价于 $(BI)C$，但不等价于 $B(IC)$。

为了便于解释，我们将使用小写英文字母 $(a \cdots z)$ 来表示子表达式。这些小写字母不会出现在实际数据中。例如，$BIC$ 可以表示为 $BxC$（即 $B\underbrace { I }_{ x }C$），$x(\underbrace {BIC}_{ x })$，$xy(\underbrace {BI}_{ x } \underbrace { C }_{ y })$，$Bxy (B\underbrace { I }_{ x }\underbrace { C }_{ y })$，但不能表示为 $Bx$。

在表达式 $pq$ 中，我们说将 $p$ 应用于 $q$。我们可以用直觉来理解，$p$ 是一个函数，而 $q$ 是它的参数。然而，求值过程与传统的计算非常不同——不是通过固定表达式树传递值，而是通过改变树结构，使得结果也是一个组合表达式。

为了求值一个表达式，我们需要选择一个子表达式，该子表达式应符合下表中的某个模式——也就是说，应该存在这样的 $x$（可能还有 $y$ 和 $z$），使得表中的模式与子表达式相等。然后我们需要将子表达式替换为表中的简化结果。

| 模式  | 简化结果 | 描述                           |
| :---: | :-------: | :-----------------------------: |
| $Bxyz$ | $x(yz)$  | 组合函数（Zusammensetzungsfunktion） |
| $Cxyz$ | $(xz)y$  | 交换函数（Vertauschungsfunktion）   |
| $Kxy$  | $x$      | 常数函数（Konstanzfunktion）       |
| $Ix$   | $x$      | 恒等函数（Identitätsfunktion）     |

替换完成后，我们必须重复这个过程，直到没有合适的子表达式为止。这个最终表达式就是原始表达式的规范形式。例如，在表达式 $CIC(CB)I$ 中，我们可以进行如下字母分配

$$\underbrace { C }_{ C }\underbrace { I }_{ x }\underbrace { C }_{ y }\underbrace {(CB)}_{ z }I$$

并看到 $CIC(CB)I ≡ (((CI)C)(CB))I ≡ (((Cx)y)z)I$ 包含了 $C$ 组合子模式，因此简化为 $((xz)y)I ≡ I(CB)CI:$

$$(\underbrace { C }_{ C }\underbrace { I }_{ x }\underbrace { C }_{ y }\underbrace { (CB) }_{ Z })I \rightarrow (\underbrace { I }_{ x } \underbrace {(CB)}_{ z }\underbrace { C }_{ y })I$$

另一个例子：$B((CK)I)IC$ 表达式。让我们先简化组合子 $B:$

$$(\underbrace { B }_{ B }\underbrace { ((CK)I) }_{ x }\underbrace { I }_{ y }\underbrace { C }_{ z } \rightarrow \underbrace { ((CK)I) }_{ x } (\underbrace { I }_{ y }\underbrace { C }_{ z }))$$

现在，让我们简化最后一个 $I:$

$$((CK)I)(\underbrace { I }_{ I } \underbrace { C }_{ x }) \rightarrow ((CK)I)C$$

最后，我们通过两次更多的简化完成求值：

$$((\underbrace { C }_{ C }\underbrace { K }_{ x }) \underbrace { I }_{ y }) \underbrace { C }_{ z } \rightarrow (\underbrace { K }_{ K }\underbrace { C }_{ x }) \underbrace { I }_{ y } \rightarrow C$$

可以证明，无论求值顺序如何，规范形式都是一样的。例如，以下求值顺序：

$$C(K(II)(\underbrace { I }_{ I }\underbrace { C }_{ x })) \rightarrow C(K(\underbrace { I }_{ I }\underbrace {  I}_{ x })(C)) \rightarrow C((\underbrace { K }_{ K }\underbrace { I }_{ x }) \underbrace { C }_{ y }) \rightarrow CI$$

和

$$C(K(\underbrace {I}_{ I }\underbrace { I }_{ x })(IC)) \rightarrow C((\underbrace { K }_{ K }\underbrace { I }_{ x })\underbrace { (IC)}_{ y }) \rightarrow CI$$

得到的结果相同。然而，如你所见，简化的次数不同：第一个情况下为 $3$ 次，第二个情况下为 $2$ 次。这提出了一个有趣的问题——找到一个给定公式所需的最小简化次数。

你的任务是编写一个程序，找到给定组合表达式求值到其规范形式所需的最小简化次数。

## 输入格式
输入文件只有一行，包含一个符合上述文法的组合表达式。表达式的长度不超过 $30 000$。表达式中不含空格或文法未指定的符号。

## 输出格式
输出一个整数——给定公式求值到规范形式所需的最小简化次数。

## 数据范围与提示
时间限制：1 秒，内存限制：256 MB。

```input1
C(K(II)(IC))

```

```output1
2

```

```input2
CIBI

```

```output2
3

```

```input3
BBBBBCCCCCKKKKKIIIII

```

```output3
15

```

## 提示
Time limit: 1 s, Memory limit: 256 MB. 




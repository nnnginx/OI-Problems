## 题目描述

Fascinated by his experience with balanced parentheses so far, Farmer John is curious if you can help him solve one final problem. As it turns out, FJ's farm is in the shape of a giant tree of  $ n $  pastures, each of which he has labeled with either ```(``` or ```)```.

For example: '('--'('--')'--'('--')' | | ')' ')'--'('--'(' | | ')' '('--')'--')'--')'--'('

Recall that since his farm is a tree, this means that certain pairs of pastures are connected by corridors so that there is one unique path between any given pair of pastures. FJ believes that some of these paths represent balanced strings of parentheses. In particular, he would like to know, among all such balanced strings represented by paths through the tree, what is the maximum nesting depth one can find. The nesting depth of a balanced string of parentheses is the maximum, over all prefixes of the string, of the excess number of ```(``` within the prefix. For example, the string ```()()()``` has nesting depth  $ 1 $ , but the string ```((()))()``` has nesting depth  $ 3 $ , as we can see clearly if we count excess ```(``` for every prefix of the string: ```((()))()``` 12321010 For the example farm above, the deepest string is ```((()))``` with a depth of  $ 3 $ , and can be obtained by taking the path from  $ A $  to  $ B $  below: '('--'('--')'--'('--')' | | ')' ')'--'('--'(' < A | | ')' '('--')'--')'--')'--'(' ^C ^B

Note that this is different than the longest balanced string; for instance ```(())(())```, starting at  $ A $  and ending at  $ C $ , has length  $ 8 $ . Your task is to output the nesting depth of the deepest balanced path in the tree.

## 输入格式

Line 1: A single integer  $ n $, the number of nodes in the tree.

Lines 2..n: Line i+1: A single integer  $ p_{i+1} (1 \leq p_{i+1} \leq i) $ , denoting an edge between nodes  $ i+1 $  and  $ p_{i+1} $  in the tree.

Lines n+1..2n: Line N+i: Either ```(``` or ```)```, the label of node  $ i $ .

## 输出格式

Line 1: A single integer, giving the maximum nesting depth of a balanced path.

## 样例输入

```
15
1
2
1
4
4
6
7
5
9
9
11
12
13
14
(
)
)
(
)
)
(
)
(
(
(
)
)
)
(
```

## 样例输出

```
3
```

## 数据规模与约定

对于 $100\%$ 的数据， $ 1 \leq n \leq 4\times 10^4 $ 。

## 题目来源

Gold


# AT_jag2018summer_day2_e Self-contained

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2018summer-day2/tasks/jag2018summer_day2_e

Ao loves certain sets of non-negative integers.

Let $ X $ be a set of non-negative integers. Whether she loves $ X $ or not is determined as follows:

- If $ X $ is the empty set, she loves $ X $.
- If, for any (possibly the same) two elements $ u $ and $ v $ in $ X $, at least one of $ u+v $ and $ {\rm\ abs}(u-v) $ is contained in $ X $, she loves $ X $.
- If none of the above conditions is satisfied, she does not love $ X $.

You are a big fan of Ao, and going to present her a set of non-negative integers. Currently you have a set $ A $ of non-negative integers. You want to erase (possibly zero) elements from $ A $ so that she loves the set of remaining integers. You also want to maximize the number of remaining integers. What is the largest number of remaining integers?

## 输入格式

Input is given from Standard Input in the following format:

> $ S $

Here, $ S=S_0S_1...S_{|S|-1} $ is the string which indicates $ A $. For each $ i $ ( $ 0\ \leq\ i\ \leq\ |S|-1 $ ), $ S_i\ = $ `1` if $ A $ contains $ i $ and $ S_i\ = $ `0` if not. It is guaranteed that $ S_{|S|-1} $ is `1`.

## 输出格式

Print the largest number of remaining integers.

## 输入输出样例 #1

### 输入 #1

```
1000001001011
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
10110110101
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
0111
```

### 输出 #3

```
0
```

## 说明/提示

### Constraints

- $ A $ is not empty.
- The largest element in $ A $ is not larger than $ 500,000 $

### Sample Explanation 1

The set $ A\ =\ \{0,6,9,11,12\} $. If you erase $ 9 $ and $ 11 $, Ao loves the set of remaining integers: $ \{0,6,12\} $.

### Sample Explanation 3

The set of remaining integers must be empty.
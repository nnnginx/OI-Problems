# AT_code_thanks_festival_14_qualb_h しりとりゲーム

## 题目描述

最近，你迷上了一种略显特殊的接龙游戏，并为此购入了一套包含多个英文单词的「接龙基础套装」。

游戏的规则如下：

- 游戏中只能使用事先规定好的单词，使用其他单词是不允许的。然而，你可以选择将一个英文单词反向后作为替代品来使用。
- 一旦某个英文单词被使用（包括其反向形式），就不能再使用了。
- 第一次发言时，可以自由选择一个英文单词。
- 从第二次发言开始，选择的英文单词的首字母必须与上一个单词的尾字母相同。
- 当无法找到符合以上条件的单词来发言时，接龙游戏立即结束。

通常，接龙游戏是多人参与的，但偏爱独处的你想尝试在一局游戏中用完所有英文单词，并结束游戏。经过推理，你发现仅靠「接龙基础套装」中的单词很可能无法实现这个目标。

因此，你打算购买额外的单词来完成接龙游戏。请找出你至少需要购买多少个额外单词。

幸运的是，在你生活的世界里，你可以购买到任何数量的英文单词。

注意：问题中提到的英文单词是由小写字母（`a`-`z`）组成，长度在 $2$ 到 $20$ 之间的字符串。这可能与真实的英文单词定义有所不同。

## 输入格式

输入由标准输入提供，格式如下：

> $ N $  
> $ w_1 $  
> $ w_2 $  
> ...  
> $ w_N $  

- 第 $1$ 行包含一个整数 $N\ (1 \leq N \leq 100,000)$，表示「接龙基础套装」中的单词数量。
- 接下来的 $N$ 行中，第 $i$ 行提供一个单词 $w_i\ (2 \leq |w_i| \leq 20)$，该单词仅由小写字母组成。
- 所有单词都是独一无二的，并且没有哪个单词的反向形式与其他单词相同。

## 输出格式

输出只需一行，表示你至少需要购买的额外单词数量。记得在行尾加上换行符。

## 输入输出样例 #1

### 输入 #1

```
3
soup
peas
ecir
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
4
ba
bc
ca
da
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
13
ab
cd
ef
gh
ij
kl
mn
op
qr
st
uv
wx
yz
```

### 输出 #3

```
12
```

## 输入输出样例 #4

### 输入 #4

```
3
aa
xyz
zwx
```

### 输出 #4

```
1
```

## 说明/提示

### 样例解释 1

使用「接龙基础套装」中的单词无法完整用完所有单词。例如，通过购买单词 `sugar`，可以这样进行接龙：`soup`→`peas`→`sugar`→`rice`（其中 `rice` 是 `ecir` 的反向形式）。这样，便能用尽所有单词，达到目标。

### 样例解释 2

比如可以这样接龙：`ab`→`bc`→`ca`→`ad`，在这种情况下，你不需要额外购买任何单词。例子中，`ba` 和 `da` 是反向使用的。

 **本翻译由 AI 自动生成**
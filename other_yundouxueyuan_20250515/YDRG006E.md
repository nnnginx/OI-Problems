# 题目背景

前排提示：某些神奇的逃课做法已经被 ban 掉了~

《编译原理》是一门非常有意思的课程。整门课程的意义在于：教你如何写一个编译器。其中涉及了很多精妙的算法、有趣的设计和伟大的灵魂(e.g. [Mr. Knuth](https://en.wikipedia.org/wiki/Donald_Knuth)) 。

我们当然希望正在做题的你，也能在 OI 这方乱世中领略到一些编译器的美。当然，千里之行，始于足下。所以，我们的挑战，将会是以渐进式的方式来进行。

To be continued ... !

# 题目描述

本题是【花式编译】的 #2 题。

小花稀里糊涂地给 6 月 S 的 A 题投了一个大模拟，太抽象了！经过一番反思，他发现了问题所在：位置放错了！

> “……其实大家还是很喜欢大模拟的，都超爱！只不过放 A 太抽象了。下次放靠后一点就合理了吧！……”

以上为当事人的结案陈词节选。不知道你信不信，反正我是信了。

Anyway，让我们说正事。本题的任务比起[花式编译 #1 成为初级表达式大师](https://yundouxueyuan.com/p/YDRS007A)更近了一步：你需要处理一些**复杂的逻辑**了。在[花式编译 #1 成为初级表达式大师](https://yundouxueyuan.com/p/YDRS007A) 的需求基础上，本题中增添了如下复杂逻辑：

- 代码存在多余空行。
- 变量名的长度可能会 $> 1$。
- 存在 `if () ... else ...` 逻辑。
- 存在 `while () ...` 逻辑。
- 增添了运算符：位运算 `&`，`|`，`^`。

例如，最终你很可能接收到形如以下格式的输入：

```cpp
int main() {
    int awa = 5 ;
    int bwb = 3 ;
    int cwc = 2 ; 
    int dwd = 1 ; 

    while (awa >= 0){
      awa = awa - 1 ; 
      bwb = bwb + (awa | (cwc ^ dwd)) * bwb ; 
      printTheRes(awa - bwb) ; 
    }
    
    return 0 ;
}
```

其中，`printTheRes()` 函数是一个**默认预设函数**，可以理解为是一个用于**输出表达式结果**的超级输出函数。代码中默认可以直接调用这个函数。具体用法上， `printTheRes(X)` 和 `cout << (X) << endl` 在语义上是等价的，其中 X 是符合题目要求的**合法表达式**。

以下是对于本题输入代码的具体细节，请仔细阅读：

- 第一行依旧是 `int main()` 声明主函数，**不保证**大括号不会换行。
- `main()` 函数中，对变量的声明是**集中的**，但声明时不一定同时给出定义。
  - 变量声明语句只会出现在 `main()` 函数的开头部分（前几行），不会出现一部分执行语句后面又出现变量声明语句的情况。同时，保证所有变量的声明都是 `int` 类型声明。
  - `main()` 函数中最开始的几句话一定是形如 `int xyz. ..` 的语句，且保证不会出现逗号 `,`。
  - 以下这个例子可能会帮助你理解一些边界条件：

```cpp
int main() {
    int xyz = 5 ;
    int ahahah ; 
    int yundou = (xyz + 114514) ^ 1919810 ;

    ...
    ahahah = yundou | 114514 ;
    ...
}
```

- 变量名保证是**仅**由**大小写字母**组成的字符串。
  
- 表达式格式：
  - 本题的测试数据中，给出的表达式一定是在 C 语言中可以直接计算的完整表达式。
  - 表达式中**包含变量名和数字**。
  - 本题的测试数据中**会出现括号 `()`**。
  - 本题的是数据中会包含以下运算符： `+`，`-`  ，`*`，`/` ，`%` ，`<` ，`>` ， `>=`，`<=`  ，`!=`，`==`，`&`，`|`，`^`。
  - 保证表达式的语法是正确的。
- 条件逻辑 if
  - 在本题中，保证只会包含如下两种形式的分支语句：
  - `if (...) { \\ do something }`。
  - `if (...) { \\ do something } else { \\ do something }`。
  - 换句话说，要么没有 `else`，要么只有一个 `else`。不存在 `else if` 语句。
  - `(...)` 可能是复杂的表达式。
  - 保证分支后执行的语句块一定被 `{}` 包裹，同时 ` \\ do something ` 部分可能包含多条语句。
  
- 条件循环逻辑 while
  - 在本题中，保证只会包含如下形式的循环语句：
  - `while (...) { \\ do something }`。
  - `(...)` 可能是复杂的表达式。
  - 保证循环的执行语句块一定被 `{}` 包裹，，同时 ` \\ do something ` 部分可能包含多条语句。

- 综上，语句块中以及 `main()` 函数中，只会存在如下语句：
  - 变量声明语句 `int yundou = 666 ;`
  - 赋值语句 `yundou = (yundou ^ 114514) * 1919 / 810`。
  - 条件语句 `if` 或循环语句 `while`。

- 我们不能限制程序员的 coding 喜好，对吧？本题的测试数据中，会存在一些不影响代码本身正确性的**多余空格或者换行**。这部分可能会对你的算法存在一定影响。也就是说，你需要为以下代码风格做好准备：

```cpp
int main() 

{
    int a =         
  
  
  
  
  
  5 ;
    int      b       =        4 ;




  
    int c =      3       ;
    int d =      
  
  2 ;
    int        e =   
  1 ;
    printTheRes(a *             b + c - d /            e) ; 

}
```

最后，给出的代码在补足缺省函数实现的前提下，保证是**能够直接在 C 语言编译环境中正确运行的代码**。

# 输入输出格式

## 输入

一个 C 语言程序。具体的输入格式参考【题目描述】中的详细解释。

## 输出

这个程序的运行结果。

# 样例

```input1
int main() {
    int a = 5;
    int b = 4;
    if (a <= b) {
        printTheRes(a);
    }

    printTheRes(b);
    return 0;
}
```

```output1
4
```

```input2
int main() {
    int a = 5;

    if (a % 2 == 0) {
        printTheRes(114514);






    } else {
        printTheRes(1919810);
    }
    return 0;
}
```

```output2
1919810
```

```input3
int main() {
    int i = 0;
    int j = 114514;
    while (i < 3) {
        j = 0;

        while (j < 2) {
            printTheRes(i * 10

+ j);
            j





= j + 1;
        }
        i = i + 1;
    }
    return 0;
}

```
```output3
0
1
10
11
20
21
```
```input4
int main() {
    int kuf;
    int hgbahjkf;
    int or;
    int and;
    int xor;

    kuf = 114;
    hgbahjkf = 514;
    or = kuf | hgbahjkf;
    and = kuf & hgbahjkf;
    xor = kuf ^ hgbahjkf;
    printTheRes(or);
    printTheRes(and);
    printTheRes(xor);
    return 0;
}
```

```output4
626
2
624
```

```input5
int main() {
  int vara;
  int varb;
  int le;
  int lt;
  int ge;
  int gt;
  int ne;
  int eq;

  vara = 114;
  varb = 514;
  le = vara <= varb;
  lt = vara < varb;
  ge = vara >= varb;
  gt = vara > varb;
  ne = vara != varb;
  eq = vara == varb;
  printTheRes(vara);
  printTheRes(varb);
  printTheRes(le);
  printTheRes(lt);
  printTheRes(ge);
  printTheRes(gt);
  printTheRes(ne);
  printTheRes(eq);
  return 0;
}
```

```output5
114
514
1
1
0
0
1
0

```


# 数据范围

对于前 $20\%$ 的数据，保证不存在 `if` 或者 `while` 逻辑。

对于前 $30\%$ 的数据，保证不存在 `while` 逻辑，且 `if` 逻辑不会嵌套。

对于前 $40\%$ 的数据，保证 `if`，`while` 逻辑均不会嵌套。

对于另外 $10\%$ 的数据，保证只存在  `+`，`-`  ，`==`，`!=` 四种运算符。

对于另外 $10\%$ 的数据，保证只存在  `+`，`*`，`>`，`<` 四种运算符。

对于另外 $20\%$ 的数据，保证代码中不存在无意义空行，且全部语法快的大括号均不换行。

对于全部 $100\%$ 的数据，保证全部中间运算结果均不超过 `INT_MAX`，全部的变量名长度均 $ < 100$，总代码长度不会超过 1KB，`If/While` 嵌套总层数 $\leq 5$ 且至多循环 $5000$次，同时只存在以下运算符：  `+`，`-`  ，`*`，`/` ，`%` ，`<` ，`>` ， `>=`，`<=`  ，`!=`，`==`，`&`，`|`，`^`。

注意：作为输入数据的 C 语言代码中，可能存在多余但不影响语义的空格或者换行。

注意 2：代码中出现的全部 `-` 均指代**二元运算**。



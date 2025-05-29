## 题目背景
欢迎参加 FAOI-R4！

小 M 作为 A 题的出题人，想要进入 A 题，从而查看选手的提交。可是小 M 不经常使用洛谷，所以他并不知道如何找到 A 题。于是很快，另一个 FAOI 团员小 L 给小 M 发了一份 A 题的题号，通过题号小 M 就可以找到 A 题。

但是，小 M 实在不会使用洛谷——他甚至不知道如何通过题号跳转到对应的题目！

## 题目描述
最终，小 M 在洛谷主界面找到了一个叫「问题跳转」的功能。在输入框内输入题号，即可跳转到对应的题目。题目的网址为 `https://www.luogu.com.cn/problem/<PID>`，其中 `<PID>` 部分是用户输入的题号。

洛谷的题号有特殊的规律：
- 第一个字符只会是 `PBCASUT` 中的一个，所有字符都是 ASCII 码在 $[33,126]$ 中的可见字符。
- 第一个字符是 `P` 的题目为「主题库题」，这类题目的题号由 `P` 加一串数字组成，如 `P1145` 和 `P10000`。

当用户输入的题号是「主题库题」时，开头的这个 `P` 可以省略。如输入 `1001` 可以跳转到 P1001。

给定小 M 输入的题号，请输出对应的网址。

## 输入格式
第一行一个正整数 $T$，表示数据组数。

对于每组数据，输入一行一个字符串，表示小 M 输入的题号。

## 输出格式
对于每组数据，输出一行一个字符串，表示对应题目的网址。

```input1
9
1001
P1234
B2027
U76533
T512682
CF10A
AT_abc114_d
SP11470
UVA13277
```

```output1
https://www.luogu.com.cn/problem/P1001
https://www.luogu.com.cn/problem/P1234
https://www.luogu.com.cn/problem/B2027
https://www.luogu.com.cn/problem/U76533
https://www.luogu.com.cn/problem/T512682
https://www.luogu.com.cn/problem/CF10A
https://www.luogu.com.cn/problem/AT_abc114_d
https://www.luogu.com.cn/problem/SP11470
https://www.luogu.com.cn/problem/UVA13277
```

## 提示
#### 【样例解释】

对于第一组数据，`1001` 实际是 `P1001` 省略的开头的 `P`，故应该输出 `https://www.luogu.com.cn/problem/P1001`。

对于第二组数据，`P1234` 没有任何省略，故应该输出 `https://www.luogu.com.cn/problem/P1234`。

#### 【数据规模与约定】

**本题开启子任务捆绑测试。**

- Subtask 1（50 pts）：字符串首字符一定不是数字。
- Subtask 2（50 pts）：无特殊限制。

对于所有数据，$1\le T\le 10$，保证输入的题号（曾经）真实存在且长度不超过 $100$ 个字符。保证输入的题号仅包含 ASCII 码在 $[33,126]$ 中的可见字符。


## 题目描述

16 世纪法国外交家 Blaise de Vigenère 设计了一种多表密码加密算法——Vigenère 密码。Vigenère 密码的加密解密算法简单易用，且破译难度比较高，曾在美国南北战争中为南军所广泛使用。

在密码学中，我们称需要加密的信息为明文，用 $M$ 表示；称加密后的信息为密文，用 $C$ 表示；而密钥是一种参数，是将明文转换为密文或将密文转换为明文的算法中输入的数据，记为 $K$。在 Vigenère 密码中，密钥 $K$ 是一个字符串，$K = k_1k_2 \dots k_n$。当明文 $M = m_1m_2 \dots m_n$ 时，得到的密文 $C = c_1c_2 \dots c_n$，其中 $c_i = m_i ® k_i$，运算 $®$ 的规则如下表所示： 

![vigenere.png](./456/file/vigenere.png)

Vigenère 加密在操作时需要注意：

1. $®$ 运算忽略参与运算的字母的大小写，并保持字母在明文 $M$ 中的大小写形式；
2. 当明文 $M$ 的长度大于密钥 $K$ 的长度时，将密钥 $K$ 重复使用。

例如，明文 $M = \text{Helloworld}$，密钥 $K = \text{abc}$ 时，密文 $C = \text{Hfnlpyosnd}$。

| 明文 | $\text{H}$ | $\text{e}$ | $\text{l}$ | $\text{l}$ | $\text{o}$ | $\text{w}$ | $\text{o}$ | $\text{r}$ | $\text{l}$ | $\text{d}$ |
|------|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 密钥 | $\text{a}$ | $\text{b}$ | $\text{c}$ | $\text{a}$ | $\text{b}$ | $\text{c}$ | $\text{a}$ | $\text{b}$ | $\text{c}$ | $\text{a}$ |
| 密文 | $\text{H}$ | $\text{f}$ | $\text{n}$ | $\text{l}$ | $\text{p}$ | $\text{y}$ | $\text{o}$ | $\text{s}$ | $\text{n}$ | $\text{d}$ |

## 输入格式

第一行为一个字符串，表示密钥 $K$，长度不超过 $100$，其中仅包含大小写字母。  
第二行为一个字符串，表示经加密后的密文，长度不超过 $1000$，其中仅包含大小写字母。

## 输出格式

输出共 $1$ 行，一个字符串，表示输入密钥和密文所对应的明文。

```input1
CompleteVictory
Yvqgpxaimmklongnzfwpvxmniytm
```
```output1
Wherethereisawillthereisaway
```

## 数据范围与提示

对于 $100\%$ 的数据，输入的密钥的长度不超过 $100$，输入的密文的长度不超过 $10^3$，且都仅包含大小写字母。
## 题目描述
[problemUrl]: https://atcoder.jp/contests/cf17-final/tasks/cf17_final_b

すぬけ君は `a`、`b`、`c` の $ 3 $ 種類の文字のみからなる文字列 $ S $ を持っています。

回文恐怖症のすぬけ君は $ S $ の文字を自由に並び替えて、$ 2 $ 文字以上の回文を部分文字列として含まないようにしようと思いました。 これが可能かどうかを判定して下さい。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
可能な場合は `YES`、不可能な場合は `NO` を出力せよ。

## 题目大意
```cpp
有一个由'a''b''c'组成的字符串，求能否通过交换字符串中字符的位置，使得得到的字符串不包含由两个或两个以上字符组成的回文子串，输出“YES”或“NO”
```
@[chen_zhe](/space/show?uid=8457) 

@[Himself65](/space/show?uid=72813) 

```input1
abac
```

```output1
YES
```

```input2
aba
```

```output2
NO
```

```input3
babacccabab
```

```output3
YES
```

## 提示
### 制約

- $ 1\ \leq\ |S|\ \leq\ 10^5 $
- $ S $ は `a`、`b`、`c` 以外の文字を含まない。

### Sample Explanation 1

このままだと `aba` という回文を含みますが、例えば `acba` のように並び替えると $ 2 $ 文字以上の回文を含まなくなります。


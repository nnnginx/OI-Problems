## 题目描述
[problemUrl]: https://atcoder.jp/contests/code-festival-2017-qualb/tasks/code_festival_2017_qualb_a

りんごさんは、とある祭りに参加しようとしています。

その祭りの名称が `FESTIVAL` で終わる文字列 $ S $ として入力に与えられるので、りんごさんが何の祭りに参加しようしているのかを出力して下さい。

ただし、$ s $ の祭りの名称は $ s $ の末尾に `FESTIVAL` を $ 1 $ つだけ追加した文字列であるとします。 例えば `CODEFESTIVAL` は `CODE` の祭りです。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
りんごさんが何の祭りに参加しようしているのかを出力せよ。

## 题目大意
输入一个字符串，请它的把后八位字符删去，再输出

感谢@RioBlu的翻译

```input1
CODEFESTIVAL
```

```output1
CODE
```

```input2
CODEFESTIVALFESTIVAL
```

```output2
CODEFESTIVAL
```

```input3
YAKINIKUFESTIVAL
```

```output3
YAKINIKU
```

## 提示
### 制約

- $ 9\ \leq\ |S|\ \leq\ 50 $
- $ S $ は大文字アルファベットのみからなる
- $ S $ は `FESTIVAL` で終わる

### Sample Explanation 1

問題文中の例の通りです。

### Sample Explanation 2

`CODEFESTIVAL` の末尾に `FESTIVAL` を追加した文字列であるので、これは `CODEFESTIVAL` の祭りとなります。


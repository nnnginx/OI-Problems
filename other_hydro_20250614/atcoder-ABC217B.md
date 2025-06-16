## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc217/tasks/abc217_b

AtCoder では現在、 `ABC` , `ARC` , `AGC` , `AHC` の $ 4 $ つのコンテストが定期的に開催されています。

AtCoder で現在定期的に開催されているコンテストは $ S_1 $ , $ S_2 $ , $ S_3 $ とあと $ 1 $ つは何ですか?

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S_1 $ $ S_2 $ $ S_3 $

## 输出格式
答えを出力せよ。

## 题目大意
有 $4$ 个字符串，分别是 "ABC" "AGC" "ARC" 和 "AHC" ，现在给出了其中的 $3$ 串，请你编程输出剩下的那一串。

```input1
ARC
AGC
AHC
```

```output1
ABC
```

```input2
AGC
ABC
ARC
```

```output2
AHC
```

## 提示
### 制約

- $ S_1 $ , $ S_2 $ , $ S_3 $ はそれぞれ、 `ABC` , `ARC` , `AGC` , `AHC` のいずれかである。
- $ S_1 $ , $ S_2 $ , $ S_3 $ は相異なる。

### Sample Explanation 1

`ARC` , `AGC` , `AHC` の $ 3 $つが入力として与えられているので、 残りの $ 1 $ つは`ABC` です。


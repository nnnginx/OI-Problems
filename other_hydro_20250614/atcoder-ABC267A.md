## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc267/tasks/abc267_a

ある日、学校へ行くのに疲れてしまった高橋くんは、土曜日まであと何日あるかを知りたくなりました。  
 その日は平日で、曜日を英語で表すと $ S $ だったことが分かっています。その日より後の直近の土曜日は何日後かを求めてください。

なお、月曜日、火曜日、水曜日、木曜日、金曜日はそれぞれ英語で `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday` です。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを整数として出力せよ。

## 题目大意
输入一个日期，问还有几天到达下个星期六。

```input1
Wednesday
```

```output1
3
```

```input2
Monday
```

```output2
5
```

## 提示
### 制約

- $ S $ は `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday` のいずれかである

### Sample Explanation 1

この日は水曜日なので、$ 3 $ 日後に土曜日になります。


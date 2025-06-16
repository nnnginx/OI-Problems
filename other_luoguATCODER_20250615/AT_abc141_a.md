# AT_abc141_a [ABC141A] Weather Prediction

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc141/tasks/abc141_a

高橋君の住む町の天気は、一日ごとに晴れ(`Sunny`)、くもり(`Cloudy`)、雨(`Rainy`)、晴れ、くもり、雨、… と周期的に変化します。

今日の天気を表す文字列 $ S $ が与えられるので、明日の天気を予測してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

明日の天気を入力と同じ形式で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
Sunny
```

### 输出 #1

```
Cloudy
```

## 输入输出样例 #2

### 输入 #2

```
Rainy
```

### 输出 #2

```
Sunny
```

## 说明/提示

### 制約

- $ S $ は `Sunny`, `Cloudy`, `Rainy` のいずれかである

### Sample Explanation 1

高橋くんの住む町では、晴れの日の次の日の天気はくもりです。
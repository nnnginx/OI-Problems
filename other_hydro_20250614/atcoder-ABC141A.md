## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc141/tasks/abc141_a

高橋君の住む町の天気は、一日ごとに晴れ(`Sunny`)、くもり(`Cloudy`)、雨(`Rainy`)、晴れ、くもり、雨、… と周期的に変化します。

今日の天気を表す文字列 $ S $ が与えられるので、明日の天気を予測してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
明日の天気を入力と同じ形式で出力せよ。

## 题目大意
高桥君居住的城市，每一天的天气都会周期性地变化为晴天（Sunny）、阴天（Cloudy）、雨（Rainy）、晴天、阴天、雨。

给出表示今天天气的字符串S，请预测明天的天气。

```input1
Sunny
```

```output1
Cloudy
```

```input2
Rainy
```

```output2
Sunny
```

## 提示
### 制約

- $ S $ は `Sunny`, `Cloudy`, `Rainy` のいずれかである

### Sample Explanation 1

高橋くんの住む町では、晴れの日の次の日の天気はくもりです。


# AT_arc005_1 [ARC005A] 大好き高橋君

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc005/tasks/arc005_1

 高橋君は自分が大好きなので、自分の評判を調べるために自分の名前が入っているツイートを調べたいと考えました。しかし彼のフォロー数は多いので、タイムラインを $ 1 $ つずつ確認して自分に関係あるつぶやきを探すのは面倒です。  
  
 そこで高橋くんを手伝うために、与えられる文から高橋君を表す単語が現れる回数を数えてください。  
 ただし、単語の一部に高橋君を表す単語を含んでいた場合も、高橋君を表す単語と完全に一致しない限り、その単語を高橋君を表す単語として数えないでください。  
  
 以下の3単語が高橋君を表す単語です。

- TAKAHASHIKUN（高橋君をヘボン式ローマ字にして、全て大文字にしたもの）
- Takahashikun（高橋君をヘボン式ローマ字にして、先頭の $ 1 $ 文字のみ大文字、残りは小文字にしたもの）
- takahashikun（高橋君をヘボン式ローマ字にして、全て小文字にしたもの）
 
 入力は以下の形式で標準入力から与えられる。 > $ N $ $ w_{0} $ $ w_{1} $ … $ w_{N-1} $.

- 入力は $ 2 $ 行ある。
- $ 1 $ 行目には、$ 2 $ 行目に与えられる文に含まれる単語数を表す整数 $ N(1≦N≦50) $ が与えられる。
- $ 2 $ 行目には $ 2 $ 文字以上 $ 100 $ 文字以下の $ 1 $ 文が与えられる。 
  - 文は単語 $ w_i(0≦i≦N-1) $から成り、各単語は空白で区切られている。
  - 最後の単語 $ w_{N-1} $ の後には空白を挟まず `.` がある。
  - 単語 $ w_{i}(0≦i≦N-1) $ は英字(`A-Z`, `a-z`)で成り立っている。

 与えられた文の中で高橋君を表す単語が現れる回数を標準出力に $ 1 $ 行で出力せよ。  
 なお、最後には改行を出力せよ。 ```

5
Takahashikun is not an eel.
```

 ```

1
```

- Takahashikun が $ 1 $ 回現れます。
 
```

5
TAKAHASHIKUN loves TAKAHASHIKUN and takahashikun.
```

 ```

3
```

- TAKAHASHIKUN が $ 2 $ 回、takahashikun が $ 1 $ 回現れるので $ 2+1=3 $ が答えです。

```

6
He is not takahasikun but Takahashikun.
```

 ```

1
```

- Takahashikun が $ 1 $ 回現れます。
- takahasikun は takahashikunではないので、高橋君を表す単語ではありません。
 
```

1
takahashikunTAKAHASHIKUNtakahashikun.
```

 ```

0
```

- 単語の一部に高橋君を表す単語が含まれていても、高橋くんを表す単語そのものでなければ当てはまりません。
 
```

18
You should give Kabayaki to Takahashikun on July twenty seventh if you suspect that he is an eel.
```

 ```

1
```

- Takahashikun が $ 1 $ 回現れます。

## 输入格式

无

## 输出格式

无
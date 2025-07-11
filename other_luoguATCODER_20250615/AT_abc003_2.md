# AT_abc003_2 [ABC003B] AtCoderトランプ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc003/tasks/abc003_2

AtCoder社では $ 1 $ 人で行うトランプを使ったゲームが流行っています。  
 AtCoder社特製トランプでは、各カードにアルファベット小文字 $ 1 $ 文字（`a`～`z`）、または`@`の文字が書かれています。  
  
 ゲームは以下の手順で行います。

1. カードを同じ枚数ずつ $ 2 $ 列に並べて文字列を $ 2 $ つ作ります。
2. `@`のカードは、それぞれ`a`,`t`,`c`,`o`,`d`,`e`,`r`のどれかのカードと置き換えます。
3. $ 2 $ つの列が指し示す文字列が同じであれば勝ち、同じでなければ負けです。
 
 手順 1. で並べられた $ 2 $ つの列が指し示す2つの文字列与えられるので、適切に`@`を置き換えて、このゲームで勝つことができるかどうかを判定するプログラムを書いてください。  
 入力は以下の形式で標準入力から与えられる。 > $ S $ $ T $

1. $ 1 $ 行目には、$ 1 $ 列目のトランプが表す文字列 $ S $ が与えられる。
2. $ 2 $ 行目には、$ 2 $ 列目のトランプが表す文字列 $ T $ が与えられる。
1. $ S $、$ T $ ともにアルファベット小文字、および、`@`のみから構成されることが保証される。
2. $ S $、$ T $ の文字数は等しく、$ 1 $ 文字以上、$ 10 $文字以下であることが保証される。
 

 このゲームで勝つことが可能であれば`You can win`と、不可能であれば`You will lose`と（シングルクォーテーションを除いて）$ 1 $ 行で出力せよ。 また、出力の末尾には改行を入れること。 ```

ch@ku@ai
choku@@i
```

 ```

You can win
```

- 例えば、`@`をうまく置き換えることによって、両方とも`chokudai`と一致させることが可能です。
 
```

aoki
@ok@
```

 ```

You will lose
```

- $ 4 $ 文字目において、`@` で `i` を置き換えることができないので、一致させることができません。
 
```

arc
abc
```

 ```

You will lose
```

- $ 2 $ 文字目において、一致させることができません。

## 输入格式

无

## 输出格式

无
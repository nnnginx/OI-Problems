# AT_k2pc001_h3 お気に入りの数2(Favorite Number2)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/k2pc-hard/tasks/k2pc001_h3

**※20:31現在, この問題もセット採点がうまく動作していないようです。修正後リジャッジを行います。(恐らくテストケース毎に表示されている結果は正しいです)。ご迷惑をおかけします。**

**※20:35セット採点データを修正し、リジャッジを行いました。正解しているように見えた解答も不正解扱いになっている可能性があります。ご確認ください。ご迷惑をおかけしました。**

 $ 2 $ 以上 $ n $ 以下の正整数 $ x $ に対して, 以下の操作が許されている.

- $ x+1 $ が$ n $ 以下のとき, $ x\ +\ 1 $ を新たな $ x $ とする.
- $ \sqrt{x} $ が整数のとき, $ \sqrt{x} $ を新たな $ x $ とする.

 例えば, $ x\ =\ 2 $ のとき, $ 3 $を新しい $ x $ とすることができる.  
 $ x\ =\ 4 $ のとき, $ (2,5) $ のいずれかを新しい $ x $ とすることができる.

 そこで, kagamizは $ x=2 $ として開始し, この操作で許される全ての遷移の仕方を, 少なくともそれぞれ $ 1 $ 回ずつ以上行って 再び $ x=2 $ に戻ってくるような方法のうち, 操作回数が最小になる場合にかかる操作回数を知りたい.  
 あなたの仕事は, そのような方法が存在するかどうかと, 存在するならばその最小操作回数をkagamizに教えてあげることである.

> $ n $

 入力では, 整数 $ n $ が $ 1 $ つだけ与えられる. 最小となる操作回数を出力せよ.  
 もし, そのような方法が存在しない場合は`-1`を出力せよ.  
 もしどのような操作も許されていない場合, 一切操作を行わなくても "この操作で許される全ての遷移の仕方を, 少なくともそれぞれ $ 1 $ 回ずつ以上行った", とみなしてよい. - $ 2\ ≦n\ ≦\ 10^{12} $ たどり着ける数の上限値
 
```

9
```

 ```

10
```

 ```

5
```

 ```

-1
```

 ```

4
```

 ```

3
```

## 输入格式

无

## 输出格式

无
# AT_agc044_d [AGC044D] Guess the Password

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc044/tasks/agc044_d

**これは対話式の問題です。**

あなたの課題は、秘密のパスワード $ S $ を当てることです。 パスワードは長さ $ L $ 以下の空でない文字列であり、パスワードの各文字は英小文字 (a, b, ..., z)、英大文字 (A, B, ..., Z)、数字 (0, 1, ..., 9) のいずれかです。

秘密のパスワード $ S $ を当てるために、クエリを送ることができます。 クエリは、上述のパスワードの要件を満たす文字列 $ T $ からなり、送られたクエリに対しては $ S $ と $ T $ の編集距離 (考慮する操作は文字の削除、挿入、置換) が回答されます。 送ることができるクエリの数は $ Q $ 個までです。

**注記**: 編集距離 (考慮する操作は文字の削除、挿入、置換) の定義については、[Wikipedia 内のこちらのページ](https://en.wikipedia.org/w/index.php?title=Levenshtein_distance&oldid=954598393) を参照してください。

### Input &amp; Output Format

クエリを送るには、標準出力に以下のように出力せよ (末尾に改行を入れること)。

> ? $ T $

ここで、文字列 $ T $ はパスワードの要件を満たさなければならない。

クエリへの回答 $ ans $ は、標準入力から以下の形式で与えられる。

> $ ans $

秘密のパスワード $ S $ を特定したら、標準出力に以下のように出力せよ (末尾に改行を入れること)。

> ! $ S $

そして、すぐにプログラムを終了させよ。

## 输入格式

无

## 输出格式

无

## 说明/提示

### 制約

- $ L\ =\ 128 $
- $ Q\ =\ 850 $
- 秘密のパスワード $ S $ は、プログラムとジャッジの対話の開始前に選ばれる。

### 判定

- **出力のたびに標準出力を flush せよ。** これが守られない場合、ジャッジ結果が `TLE` となる可能性がある。
- 秘密のパスワード (とあなたが考えるもの) を出力したら、直ちにプログラムを終了させよ。これが守られない場合のジャッジ結果は未定義である。
- 不正な形式のクエリが送られた場合 (例: 送られた文字列がパスワードの要件を満たさない、出力の先頭に `?` がない)、プログラムが異常終了した場合、または $ Q $ 回を超えてクエリが送られた場合のジャッジ結果は未定義である (`WA` とは限らない)。

### 入出力例

以下の例において、秘密のパスワードは `Atcod3rIsGreat` です。

 Input Output  $ \texttt{?\ AtcoderIsBad} $ $ 5 $   $ \texttt{?\ AtcoderIsGreat} $ $ 1 $   $ \texttt{!\ Atcod3rIsGreat} $
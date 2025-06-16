# AT_tenka1_2013_qualB_a 天下一人力比較

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2013-qualb/tasks/tenka1_2013_qualB_a

下記の文字列が標準入力から与えられる。問題文においてカズキ君の渡された文字列と同じである。

 ```

ABGGEGBCFEBFBAF
FFGFACCCECDGCDGAFFFACGDA
EEDCAEAFBDDEEDGGA
GDCAGFFAACBGEDBAFBCDECGAE
EDB
GADGADEDBCGABDDCBBDBEAD
GADBB
DFCE
BFGCGCBEDC
EDGADBGGDDFEEGGFDGCAFBFGFAAD
DDAEBGACDFDGDAB
EEDCECFFAE
ADDBEEABFEAB
FEEBFDGAADAE
GB
```

 辞書順比較で $ 7 $ 番目に小さい文字列を標準出力に $ 1 $ 行で出力せよ。  
 なお、行の終端には改行が必要である。

## 输入格式

无

## 输出格式

无

## 说明/提示

### 辞書順比較について

 天下一株式会社に勤めるカズキ君は、以下の文字列の中から辞書順比較で $ 7 $ 番目に小さいものを選ぶという仕事を言い渡された。

 あなたは唖然とするカズキ君を助けるためにプログラムを書いて、答えを見つけることにした。

- ABGGEGBCFEBFBAF
- FFGFACCCECDGCDGAFFFACGDA
- EEDCAEAFBDDEEDGGA
- GDCAGFFAACBGEDBAFBCDECGAE
- EDB
- GADGADEDBCGABDDCBBDBEAD
- GADBB
- DFCE
- BFGCGCBEDC
- EDGADBGGDDFEEGGFDGCAFBFGFAAD
- DDAEBGACDFDGDAB
- EEDCECFFAE
- ADDBEEABFEAB
- FEEBFDGAADAE
- GB

- - - - - -

 文字列 $ A $ に対して、 $ A_i $ で $ i $ 番目の文字を表し、 $ |A| $ で文字列 $ A $ の文字数を表すことにすると、文字列 $ A $ と文字列 $ B $ を辞書順比較で比較するとは、

- $ A_i\ \neq\ B_i $ となる最小の $ i $ $ (1\ \leq\ i\ \leq\ {\rm\ min}(|A|,\ |B|)) $に対して
- $ A_i\ であれば、文字列\ A $ は文字列 $ B $ より小さい
- $ A_i\ >\ B_i $ であれば、文字列 $ A $ は文字列 $ B $ より大きい

- そのような $ i $ が存在しなければ、文字数が少ない方を小さいとする

 として文字列 $ A $ と文字列 $ B $ の大小関係を決めることである。

 なお、アルファベットの大小関係は、 `A` $ \lt{} $ `B` $ \lt{} $ `C` $ \lt{} $ $ ... $ $ \lt{} $ `Y` $ \lt{} $ `Z` である。  
 例えば、 `AA`, `B`, `BA`, `AB`, `A` の中から辞書順比較で $ 3 $ 番目に小さいものは `AB`である。(`A` $ \lt{} $ `AA` $ \lt{} $ `AB` $ \lt{} $ `B` $ \lt{} $ `BA` である。)
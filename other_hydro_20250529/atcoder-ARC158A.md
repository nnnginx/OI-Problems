## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc158/tasks/arc158_a

屁方 $ x_1,\ x_2,\ x_3 $ が嚥えられます��あなたはこれらの屁方に��して��肝の荷恬を採業でも佩うことができます��$ 0 $ 指でもよい����

- $ (1,2,3) $ の��双 $ (i,j,k) $ をひとつ�xぶ��つまり $ 1\leq\ i,j,k\leq\ 3 $ であるような屁方の�M $ (i,j,k) $ であって $ i\neq\ j,\ i\neq\ k,\ j\neq\ k $ となるものを�xぶ��
- その瘁��$ x_i $ を $ x_i+3 $��$ x_j $ を $ x_j+5 $��$ x_k $ を $ x_k+7 $ で揖�rに崔き�Qえる��
 
あなたの朕議は��$ x_1=x_2=x_3 $ が撹り羨つようにすることです��このことが辛嬬であるか倦かを登協してください��辛嬬な��栽には��それを�_撹するための恷弌の荷恬指方を竃薦してください��

$ T $ ��のテストケ�`スが嚥えられるので��それぞれについて基えを箔めてください��

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられます��

> $ T $ $ \text{case}_1 $ $ \vdots $ $ \text{case}_T $

光テストケ�`スは參和の侘塀で嚥えられます��

> $ x_1 $ $ x_2 $ $ x_3 $

## 補竃鯉塀
$ T $ 佩竃薦してください��$ i $ 佩朕には $ i $ 桑朕のテストケ�`スについて��肝の�､魍�薦してください��

- $ x_1=x_2=x_3 $ が撹り羨つようにすることが辛嬬ならば��それを�_撹するための恷弌の荷恬指方��
- $ x_1=x_2=x_3 $ が撹り羨つようにすることが音辛嬬ならば��$ -1 $��

## 籾朕寄吭
公低眉倖方 $a,b,c$��低辛參繍宸眉倖方梓販吭乏會蛍艶 $+3,+5,+7$��箔頁倦嬬聞誼恷嶮 $a=b=c$��泌惚頁補竃恷弌荷恬方��泌惚倦補竃 $-1$。

$1\le a,b,c\le 10^9$。

```input1
4
2 8 8
1 1 1
5 5 10
10 100 1000
```

```output1
2
0
-1
315
```

## 戻幣
### 崙�s

- $ 1\leq\ T\leq\ 2\times\ 10^5 $
- $ 1\leq\ x_1,\ x_2,\ x_3\ \leq\ 10^9 $
 
### Sample Explanation 1

ひとつめのテストケ�`スについて��肝のように荷恬を佩うことで $ x_1=x_2=x_3 $ が撹り羨つようにできます�� - $ (i,j,k)\ =\ (3,2,1) $ として荷恬を佩う��$ (x_1,x_2,x_3) $ は $ (9,13,11) $ に崔き�Qわる�� - $ (i,j,k)\ =\ (2,3,1) $ として荷恬を佩う��$ (x_1,x_2,x_3) $ は $ (16,16,16) $ に崔き�Qわる��


## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/s8pc-3/tasks/s8pc_3_g

肝のような方双があります。

- $ a_1=a_2=1 $, $ a_{k+2}=a_{k+1}+a_k\ (k\ \ge\ 1) $
 
  
 E869120は, この方双を聞って肝のように方双 $ d_1,\ d_2,\ d_3,\ \dots\ ,\ d_n $ を協�xすることにしました。  
- $ d_{1,\ j}\ =\ a_j $
- $ d_{i,\ j}\ =\ \sum_{k\ =\ 1}^j\ d_{i\ -\ 1,\ k}\ (i\ \ge\ 2) $
 
  
 屁方 $ n,\ m $ が嚥えられます。そのとき, $ d_{n,\ m} $ の�､鯒鵑瓩討�ださい。  
 ただし, 基えが掲械に寄きくなることがあるので, $ 998,244,353 $ で護った噫りを箔めてください。  
 あなたはこの���}が盾けますか???   
 ���}猟毅輝宀��square1001

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ n\ \quad\ m $

- 1佩朕には, 屁方 $ n,\ m $ が腎易曝俳りで嚥えられる。

## 補竃鯉塀
- $ d_{n,\ m} $ を $ 998,244,353 $ で護った噫りを箔めなさい。

## 籾朕寄吭
吭房祥頁補秘曾倖方n才m   
幹夛匯倖屈略裳專d[][] (宸倖裳專辛嬬載寄)   

及匯佩頁豎襖椎弐方双 
```
1 1 2 3 5 8 13....
```
及n佩議d[j][i]��紗貧d[j-1][i+1]誼d[j][i+1]	(耽佩遍倖方脅葎1)  
劔箭1:   
補秘:
```
4 7
```
補竃:
```
176
```
屈略裳專:
```
1 1 2 3 5 8 13...
1 2 4 7 12 20 33...//1+1=2,2+2=4,4+3=7,7+5=12...
1 3 7 14 26 46 79...//1+2=3,3+4=7,7+7=14,14+12=26...
1 4 11 25 51 97 [176](d[4][7])...
.....
.....
```
咀葎方辛嬬載寄 侭參
勣箔補竃d[n][m]貧議方mod 998,244,353

$n\le2\times10^5,m\le10^{18}。$

湖仍@ВОЛШЕБНИК 戻工議鍬咎

```input1
4 7
```

```output1
176
```

```input2
12 20
```

```output2
174174144
```

```input3
16 30
```

```output3
102292850
```

## 戻幣
### 崙�s

- $ 1\ \le\ n\ \le\ 200,000 $
- $ 1\ \le\ m\ \le\ 10^{18} $

### 弌�n�}

 弌�n�}1 \[ $ 100 $ 泣 \]

- $ 1\ \le\ n,\ m\ \le\ 3,000 $ を�困燭后�
 
 弌�n�}2 \[ $ 170 $ 泣 \]   
- $ 1\ \le\ m\ \le\ 200,000 $ を�困燭后�
 
 弌�n�}3 \[ $ 230 $ 泣 \]   
- $ 1\ \le\ n\ \le\ 3 $ を�困燭后�
 
 弌�n�}4 \[ $ 420 $ 泣 \]   
- $ 1\ \le\ n\ \le\ 1000 $ を�困燭后�
 
 弌�n�}5 \[ $ 480 $ 泣 \]   
- 弖紗の崙�sはない。
 
  
### Sample Explanation 1

參和のような方双になっています。 $ d_{i,\ 1} $ $ d_{i,\ 2} $ $ d_{i,\ 3} $ $ d_{i,\ 4} $ $ d_{i,\ 5} $ $ d_{i,\ 6} $ $ d_{i,\ 7} $ $ d_1 $ 1 1 2 3 5 8 13 $ d_2 $ 1 2 4 7 12 20 33 $ d_3 $ 1 3 7 14 26 46 79 $ d_4 $ 1 4 11 25 51 97 176 よって, $ d_{4,\ 7}\ =\ 176 $ となり, これが基えとなります。

### Sample Explanation 3

$ d_{16,\ 30}\ =\ 1,193,004,294,685 $ なので, これを $ 998,244,353 $ で護った噫りは $ 102,292,850 $ です。


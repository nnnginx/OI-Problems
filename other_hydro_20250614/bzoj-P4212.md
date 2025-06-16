## 题目描述

Hzwer 成功培育出神牛细胞，可最终培育出的生物体却让他大失所望......

后来，他从某同校女神牛处知道，原来他培育的细胞发生了基因突变，原先决定神牛特征的基因序列都被破坏了，神牛 hzwer 很生气，但他知道基因突变的低频性，说不定还有以下优秀基因没有突变，那么他就可以用限制性核酸内切酶把它们切出来，然后再构建基因表达载体什么的，后面你懂的......

黄学长现在知道了 $N$ 个细胞的 DNA 序列，它们是若干个由小写字母组成的字符串。一个优秀的基因是两个字符串 $s_1$ 和 $s_2$，当且仅当 $s_1$ 是某序列的前缀的同时，$s_2$ 是这个序列的后缀时，hzwer 认为这个序列拥有这个优秀基因。

现在黄学长知道了 $M$ 个优秀基因 $s_1$ 和 $s_2$，它们想知道对于给定的优秀基因，有多少个细胞的 DNA 序列拥有它。

## 输入格式

第一行：$N$，表示序列数。

接下来 $N$ 行，每行一个字符串，代表 $N$ 个 DNA 序列，它们的总长为 $L_1$。

接下来一个 $M$，表示询问数。

接下来 $M$ 行，每行两个字符串 $s_1'$ 和 $s_2'$，由一个空格隔开，hzwer 希望你能在线回答询问，所以 $s_1$ 等于 $s_1'$ 的所有字符按字母表的顺序向后移动 $ans$ 位（字母表是一个环），$ans$ 为上一个询问的答案，$s_2$ 同理。

例如 $ans=2,s_1'=$ `qz`，则 $s_1=$ `sb`。

对于第一个询问，$ans=0$。

$s_1$ 和 $s_2$ 的总长度为 $L_2$。

## 输出格式

输出 $M$ 行，每行一个数，第 $i$ 行的数表示有多少个序列拥有第 $i$ 个优秀基因。

## 样例
```input1
10
emikuqihgokuhsywlmqemihhpgijkxdukjfmlqlwrpzgwrwozkmlixyxniutssasrriafu
emikuqihgokuookbqaaoyiorpfdetaeduogebnolonaoehthfaypbeiutssasrriafu
emikuqihgokuorocifwwymkcyqevdtglszfzgycbgnpomvlzppwrigowekufjwiiaxniutssasrriafu
emikuqihgokuorociysgfkzpgnotajcfjctjqgjeeiheqrepbpakmlixyxniutssasrriafu
emikuqihgokuorociysgfrhulymdxsqirjrfbngwszuyibuixyxniutssasrriafu
emikuqihgokuorguowwiozcgjetmyokqdrqxzigohiutssasrriafu
emikuqihgokuorociysgsczejjmlbwhandxqwknutzgdmxtiutssasrriafu
emikuqihgokuorociysgvzfcdxdiwdztolopdnboxfvqzfzxtpecxcbrklvtyxniutssasrriafu
emikuqihgokuorocsbtlyuosppxuzkjafbhsayenxsdmkmlixyxniutssasrriafu
emikuqihgokuorociysgfjvaikktsixmhaasbvnsvmkntgmoygfxypktjxjdkliixyxniutssasrriafu
10
emikuqihgokuorociysg yxniutssasrriafu
aiegqmedckgqknky eqpoowonnewbq
xfbdnjbazhdnhkhvb qrqgbnmlltlkkbtyn
bjfhrnfedlhrlolzfv qppxpoofxcr
zhdfpldcbjf stsidponnvnmmdvap
zhdfpldcbjfpjmjxdt gdstsidponnvnmmdvap
dlhjtphgfnjtnqnbhxr wxwmhtsrrzrqqhzet
bjfhrnfedlhrlolzfv frqppxpoofxcr
zhdfpldcbjf dponnvnmmdvap
ucyakgyxweakehes nondykjiiqihhyqvk
```
```output1
4
7
3
5
5
1
3
5
10
4
```
## 数据规模与约定

对于 $100\%$ 的数据：$N\le 2\times 10^3$，$L_1\le 2\times 10^6$，$M\le 10^5$，$L_2\le 2\times 10^6$，字符串中仅包含小写字母。
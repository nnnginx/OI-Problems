## 题目背景
A 国有 $n$ 座城市，这 $n$ 座城市排成一排（编号 $1$ 到 $n$），A国的人们幸福快乐地生活着，人口呈增长很快。因此，到了天下第一的fkc IOI捧杯那年（2020年），A国的人已经多到数不清了，我们不妨假设 A 国这 $n$ 座城市每座城市中的人口都有无限个。A 国的风向很特别，始终是从 $n$ 城市吹向 $1$ 城市。A 国没有首都，在发生状况时，每个城市的政府都不会去支援其他城市。

## 题目描述
然而，在 fkc 捧杯后不久，邪恶的B国国王X制造了傻逼病毒希望以此来摧毁 A 国。A 国遭受了重大的灾难。傻逼症分一期和二期。感染了一期傻逼症的人会觉得自己是傻逼，而且希望只有自己能被称作傻逼，因此会经常大打出手，扰乱社会秩序。傻逼症二期的病人还会产生一系列的精神疾病，而且具有较强传染性。X会使用傻逼风暴来传染傻逼症，傻逼风暴会导致各种通讯工具和设备在短时间内瘫痪，因此，如果在i城爆发傻逼风暴，那么i城在傻逼风暴期间政府无法发挥很大的作用，我们不妨认为i城在傻逼风暴期间会处于无政府状态。

如果 $i$ 城市爆发 $k$ 级傻逼风暴 $(k>0) $，会导致 $i$ 城市接下来一秒有一个普通人感染二期傻逼症，如果第一秒末感染了二期傻逼症但未被隔离的人有 $x$ 个，那么第二秒感染一期傻逼症的人会增加 $c_x$ 个，感染二期傻逼症的人会增加 $d_x$ 个。（$c$，$d$ 是给定常数）。然后如果 $k$ 为 $1$ 那么该城市的傻逼风暴就会停止，政府设备又会恢复。否则该城市第三秒会继续爆发 $k-1$ 级傻逼风暴（期间政府不会恢复）。

X每次会在第 $i$ 个城市投掷 $k$ 级风暴种子，由于风向原因，$i$ 城市会爆发 $k$ 级傻逼风暴，沿风向过去后的下一个城市会爆发 $k-1$ 级傻逼风暴，再沿风向过去后的下一个城市会爆发 $k-2$ 级傻逼风暴……直至爆发的傻逼风暴等级小于 $1$ 或者再沿风向下去没有城市了。

当然，A 国各个城市的政府十分强大，不会束手就擒于傻逼症的攻击，他们会通过隔离病人以起到拖延傻逼症的蔓延速度。大佬们能在瞬间找到所有感染了傻逼症的人并将他们隔离。但是很无奈，傻逼风暴会暂时使这些设备失灵。

但是，X的风暴种子可以无限生产，无限释放。A 国政府只使用隔离法显然不是个明智的选择。于是 A 国的一些大佬开始夜以继日地尝试着研发能控制傻逼症的药物。功夫不负有心人，A 国终于研发出了治疗法术。A 国组建了联合政府，可以在城市i投放k级治疗法术，这样子，对于所有的 $\{j\mid k\ge |i-j|\}$ 城市，所有已被隔离的一期傻逼病人变成普通人，二期傻逼症病人变成一期傻逼症病人。

当然，X也十分强大，他还研制出了一种增强法术来对抗治疗法术。增强法术可使傻逼病毒更加快速地寻找宿主细胞进行繁殖，从而加重傻逼症，增加传染性。X每次会在城市 $i$ 投放 $k$ 级增强法术，那么对于所有 $\{j\mid k\ge |i-j|\}$ 的城市，所有的一期傻逼症患者变成二期傻逼症患者。而且短期内增强的傻逼病毒可依附在空气中传播，所以如果当前该城市一共有 $x$ 个傻逼症患者，那么在增强法术作用效果结束之前，该城市又会有一共 $(c+d)x$ 个普通人变成一期傻逼症患者。

由于本次事件事态十分严重，A 国联合政府的临时主席想要尽快知道患有傻逼症的病人有多少个，所以他找到了你来帮助他尽快算出答案。

所以现在给定一些事件，每一个事件都在上一个事件结算完毕之后发生：

1. 邪恶的 B 国国王X在城市 $i$ 投放了 $k$ 级风暴种子。
2. A 国联合政府在城市 $i$ 投放了 $k$ 级治疗法术。
3. X 在城市 $i$ 投放了 $k$ 级增强法术。
4. A 国联合政府想知道对于所有的 $\{k\mid l\le k\le r\}$ 城市，一共有多少个一期傻逼症病人。
5. A 国联合政府想知道对于所有的 $\{k\mid l\le k\le r\}$ 城市，一共有多少个二期傻逼症病人。

一开始 A 国没有人感染傻逼症，请对于每一个 $4,5$ 事件给出一个 A 国联合政府想要的答案，因为答案可能很大，所以你只要输出对 $998244353$ 取模后的答案即可。

## 输入格式
第一行依次输入 $4$ 个正整数 $n,m,c,d$。$m$ 表示一共有多少个事件。

接下来 $m$ 行，每行表示一个事件。

每行第一个数字 $opt$ 表示事件类型。

- 如果 $opt=1$，表示投放风暴种子，接下来两个数 $i,k$ 如题目所述。
- 如果 $opt=2$，表示投放治疗法术，接下来两个数 $i,k$ 如题目所述。
- 如果 $opt=3$，表示投放增强法术，接下来两个数 $i,k$ 如题目所述。
- 如果 $opt=4$，表示询问一期傻逼症，接下来两个数 $l,r$ 如题所述。
- 如果 $opt=5$，表示询问二期傻逼症，接下来两个数 $l,r$ 如题所述。


## 输出格式
如题所述，每个询问结果占一行。


```input1
5 4 2 3
1 3 2
1 4 2
4 1 2
5 2 4
```

```output1
2
48
```

```input2
10 8 2 8
1 7 4
3 1 4
5 1 3
2 3 5
1 6 3
5 5 8
3 6 6
4 4 7
```

```output2
0
909
94680
```

```input3
6 6 3 4
1 5 6
5 1 3
3 2 4
5 3 6
3 1 5
5 2 3
```

```output3
965
42365
13048
```

## 提示
样例 1 第一个事件中城市 $3$ 爆发 $2$ 级傻逼风暴，城市 $2$ 爆发 $1$ 级傻逼风暴。以城市 $3$ 为例，首先产生一个二期，然后增加 $2$ 个一期，再增加 $3$个二期，然后风暴变为 $1$ 级，再增加 $1$ 个二期，那么当前有 $5$ 个二期，那么又增加了 $10$ 个一期和 $15$ 个二期。所以在结算之后城市 $2$ 有 $4$ 个二期，$2$ 个一期，城市 $3$ 有 $20$ 个二期，$12$ 个一期。这些患者均被隔离，然后第二个事件城市 $3$ 增加了 $4$ 个二期，$2$ 个一期，城市 $4$ 增加了 $20$ 个二期，$12$个一期。对于第一个询问显然是 $2$。对于第二个询问，结算之后城市 $2$ 有 $4$ 个二期，城市 $3$ 有 $24$ 个二期，城市 $4$ 有 $20$ 个二期，加起来是 $48$。

本题一共五个点。

对于所有数据，$1\le c,d\le 10^7$，$1\le i,k,l,r\le n$。

第一个点：$n=1000$，$m=1000$。  
第二个点：$n=20000$，$m=20000$。  
第三个点：$n=100000$，$m=99999$，特殊性质：第一个事件为事件 $1$，之后只有事件 $3$ 和事件 $5$。  
第四个点：$n=100000$，$m=99998$，特殊性质：没有事件 $2$ 和事件 $3$。  
第五个点：$n=100000$，$m=100000$。  


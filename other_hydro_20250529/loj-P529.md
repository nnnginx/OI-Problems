## 题目描述

LOJ 停止运行后，服务商删除了网站，于是所有题目的测试数据都丢失了。

为了拯救 LOJ，LCR 要上传自己存储的比赛数据，但在放学前她都要在教室里听语法课。
然而语文老师讲课如长江大河滔滔不绝，LCR 感到十分无聊，于是便出了一道题：

> 众所周知，现代英语和汉语是 `SVO`（主谓宾）结构的语言。另外英语也有 `VO` 和 `OV` 两种常见的结构，汉语则只有 `OV` 没有 `VO` 结构。通常 `S` 和 `O` 是名词性结构，`V` 是动词性结构。

> `SVO`，`OV` 和 `VO` 整体都是名词性结构，可以嵌套。

现在已知几句话中每个词的词性（每句话是一个 `N` 和 `V`组成的字符串，`N` 表示一个名词性的词，`V` 表示一个动词性的词），请你判断每句话是否分别符合英语和汉语的结构。

符合汉语结构的字符串定义为：

* 字符串 `N` 是符合条件的。
* 把一个合法字符串中的任意一个 `N` 替换成 `NV` 或 `NVN` 得到的字符串都是符合条件的。

即：$\mathrm{N\rightarrow (NV|NVN)}$

符合英语结构的字符串是这样定义的：

* 字符串 `N` 是符合条件的。
* 把一个合法字符串中的任意一个 `N` 替换成 `NV` 或 `NVN` 或 `VN` 得到的字符串都是符合条件的。

即：$\mathrm{N\rightarrow (NV|NVN|VN)}$

## 输入格式

第一行一个正整数 $T$ 表示数据组数。

接下来 $T$ 行每行一个非空字符串 $S$ 表示要判断的字符串。

## 输出格式

输出共 $T$ 行。

每行依次输出两个空格隔开的整数 $a$ 和 $b$。

如果该字符串符合英语结构，$a=1$，否则 $a=0$；
如果该字符串符合汉语结构，$b=1$，否则 $b=0$。

```input1
3
NNV
VNVN
NVNV
```

```output1
0 0
1 0
1 1
```

## 数据范围与提示

设字符串长度的最大值为 $M$。
对于所有数据，$1\le M\le 10^6,1\le T\le 10$。

|Subtask #|分值|$M$ 的限制|特殊限制|
|:-:|:-:|:-:|:-:|
|1|$17$|$M\le 35$||
|2|$24$|$M\le 200$||
|3|$24$|$M\le 2000$||
|4|$13$|$M\le 10^5$|字符串中 `N` 不超过 $100$ 个|
|5|$22$|$M\le 10^6$|无|



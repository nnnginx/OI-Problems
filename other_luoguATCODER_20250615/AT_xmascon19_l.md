# AT_xmascon19_l Signboard 2

## 题目描述

兔子正在设计 Xmas Contest 2019 的招牌，但感到头痛不已。为了放松，她决定利用设计纸的背面来制作一个拼图。同时，她还希望这个拼图能作为一种趣味活动，供 Xmas Contest 的参赛者们进行解谜。

兔子一边设计招牌，一边用那张纸的反面创建了一个[骨架拼图](https://ja.wikipedia.org/wiki/%E3%82%B9%E3%82%B1%E3%83%AB%E3%83%88%E3%83%B3_(%E3%83%91%E3%82%BA%E3%83%AB))。不幸的是，纸张被撕成了碎片（请见 [Signboard 1](https://atcoder.jp/contests/xmascon19/tasks/xmascon19_a)），现在只剩下回忆中的拼图形状，而单词列表却分散在这些纸片上。能否想办法重新完成这份骨架拼图呢？

![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_xmascon19_l/2f961a806fdb5c0d3d6fd6d07665cf0814091861.png) 显示骨架拼图的盘面

#### 问题

根据给出的纸片信息和拼图盘面，用纸片上的单词来解决这个骨架拼图。

总共有 $64$ 张纸片，每张编号从 $1$ 到 $64$。

**可以从[这个链接](https://img.atcoder.jp/xmascon19/signboard_t2.zip)下载包含纸片信息的 zip 文件。** zip 文件中包含：

- `signboard_t2/pieces/*.txt`：存放纸片正面信息的文本文件。例如，编号为 $10$ 的纸片内容保存在 `10.txt` 中。
- `signboard_t2/pieces/p_*.png`：上述 `*.txt` 文件的图像化表示。
- `signboard_t2/pieces_back/*.txt`：存放纸片背面信息的文本文件。例如，编号为 $10$ 的纸片内容保存在 `10.txt` 中。
- `signboard_t2/skeleton.txt`：兔子回忆中的拼图盘面信息。`.` 表示不能填入字母的格子，`*` 表示可以填入字母的格子。

纸片上有解决拼图所需的所有单词，但可能也包含一些无关的笔记。你需要从中找出正确的单词来完成拼图。

## 输入格式

无

## 输出格式

输出骨架拼图的解，将 `skeleton.txt` 文件中 `*` 位置用相应的小写英文字母填充。

例如：

```
.....greet....
....m...n.....
....y...c.....
enter..free...
....i...y.....
...bagpipe..e.
....d...t.i.n.
.....a..i.n.i.
d..rigorous.g.
o....i..n.i.m.
polyglot.ideal
e....i....e...
.....t........
...keystone...
```

这样的格式符合要求。（不过请注意，这个解并非仅由纸片上的单词构成，因此会被判定为错误 `WA`）

 **本翻译由 AI 自动生成**
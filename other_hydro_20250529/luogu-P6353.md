## 题目描述
给你一个二进制的数字，请将其转换到八进制。

---

可以使用如下转换方法：

- 如果二进制的数字的位数不能被三整除，则在左侧补 $0$ 直到数字位数是 $3$ 的倍数。
- 将这个二进制数每三位分成一组。
- 每组的二进制可用如下表格所示的数字替换。

![](https://cdn.luogu.com.cn/upload/image_hosting/tcwf1oqm.png)

现在请你完成这个操作，并输出最终的八进制结果。

## 输入格式
输入一行一个二进制数。

保证位数不超过 $100$，并且首位为 $1$。

## 输出格式
输出一行一个八进制数。

```input1
1010
```

```output1
12
```

```input2
11001100
```

```output2
314
```

## 提示
#### 说明

**题目译自 [COCI2007-2008](https://hsin.hr/coci/archive/2007_2008/) [CONTEST #3](https://hsin.hr/coci/archive/2007_2008/contest3_tasks.pdf) *T2 OKTALNI***。


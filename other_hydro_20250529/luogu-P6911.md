## 题目描述
A qanat is an irrigation system widely used to deliver water in hot, arid climates. The technology was originally developed by Persians over 2000 years ago. In Morocco, qanats are known as khettara and are still used today in the southern part of the country.

The basic feature of a qanat is an essentially horizontal channel that brings water from an underground water source to an outlet near a civilization. There is also a shaft known as a mother well that rises vertically from the underground water source to the surface of a mountain or hill. Creating such a system is extremely expensive, and was especially so in ancient times, since all of the materials excavated from the channel and mother well must be carried above ground, either through the channel outlet or the top of the mother well. To aid in the construction, there are often one or more additional vertical shafts placed at strategic locations above the underground channel. Although these shafts must also be excavated, they provide a means for lifting additional dirt from the horizontal channel as illustrated in Figure 1.

  ![](https://vj.z180.cn/4dea3d690f1497e79acad3985c8a9915?v=1603314265) 

   Figure 1: An illustration of a qanat. 

For this problem, model the cross-section of a qanat as shown in Figure 2, with the channel outlet at $(0,0)$, the water source at $(w,0)$, and the top of the mother well at $(w,h)$ with $w > h$. The surface of the mountain extends along a straight line from $(w,h)$ to $(0,0)$.

  ![](https://vj.z180.cn/a58cc42544b91877083973369ca77d3c?v=1603314265) 

   Figure 2: A simplified model of a qanat cross-section. 

Every qanat must have a vertical mother well from the water source to the mountain surface above, along with $n$ additional vertical shafts. The channel and all shafts are modeled as line segments. Your goal is to determine the placement for those additional shafts so as to minimize the overall excavation cost. This cost is equal to the sum of the distances that each piece of excavated dirt must be transported to reach the surface (using any combination of horizontal and vertical movement). For example, the cost of excavating a continuous section of dirt starting from the surface and going along a path of length $\ell $ (possibly including turns) is $\int _0^{\ell } x \, dx = \frac{1}{2} \ell ^2$.

## 输入格式
The input consists of a single line containing three integers $w$ ($1 \le w \le 10\, 000$), $h$ ($1 \le h < w$), and $n$ ($1 \le n \le 1\, 000$). The value $w$ is the horizontal distance from the water source to the qanat outlet. The value $h$ is the vertical distance from the water source to the mountain surface. The value $n$ is the number of vertical shafts that must be used in addition to the mother well.

## 输出格式
First, display the minimum overall excavation cost. Next, display the $x$-coordinates, in increasing order, for $n$ optimally placed vertical shafts. If $n > 10$, display only the first $10$ $x$-coordinates. Answers within an absolute or relative error of $10^{-4}$ will be accepted. You may assume that there is a unique solution. No test case will result in a shaft within $0.001$ units from the outlet of the qanat channel or from another shaft.

## 题目大意
[原题面链接](https://icpc.global/worldfinals/problems/2015-ICPC-World-Finals/icpc2015.pdf)

### **题目描述**

qanat 是一种广泛用在气候炎热、干旱的地区中供水的灌溉系统。这项技术最初由波斯人在 $2000$ 多年前发明。在摩洛哥，qanat 被称为 khettara。至今该系统在该国南部地区仍然被使用。

qanat 的基本特点是用一个基本上是水平的沟渠，把水从地下水源带到靠近城市的出水口。还有一个被称为母井的轴垂直向上延升，从地下水源上升到山脉或山丘的地表。建设这样的系统非常昂贵，在古代更加如此，因为从沟渠和母井中挖出的所有材料都必须在地表运输。这可以通过沟渠出口或母井顶部来进行。为了帮助施工，通常在地下沟渠上方的关键位置还会放置一个或多个额外的垂直井口。尽管这些井口也必须需要被挖掘，但它们提供了一种从水平沟渠中运输额外泥土的手段，如图 $1$ 所示。

![](https://cdn.luogu.com.cn/upload/image_hosting/s71tofvr.png)

对于这个问题，模拟一个 qanat 的横截面，如图 $2$ 所示，其中通道出口在 $(0,0)$，水源在 $(w,0)$，母井顶部在 $(w,h)$，其中 $w > h$。山的表面沿着一条直线延伸，从 $(w,h)$ 到 $(0,0)$。

![](https://cdn.luogu.com.cn/upload/image_hosting/4bk00ojs.png)

每个 qanat 必须从水源到山体表面上有一个垂直的母井，还需要 $n$ 个额外的垂直井。水道和所有垂直井都被建模为线段。你的目标是确定这些额外井的位置，以最小化整体的挖掘成本。这个成本等于每块挖掘的土壤必须被运输到表面的距离的总和（任何水平和垂直运动的组合）。例如，从表面开始并沿着长度为 $l$ 的路径挖掘连续的土壤的成本为 $\int_0^l x \ \mathop{}\!\mathrm{dx}=\frac{1}{2}l^2$。

### **输入格式**

输入是一行，包含三个整数 $w$ $(1\le w\le 10000)$， $h$ $(1\le h<w)$，和 $n$ $(1\le n\le 1000)$，分别表示水源到 qanat 出口的水平距离，水源到山体表面的垂直距离和除了母井之外必须使用的垂直井口的数量。

### **输出格式**

首先，输出最小开挖成本。接下来，按照递增顺序输出 $n$ 个最优放置的竖井的 $x$ 坐标。如果 $n > 10$，则仅输出前 $10$ 个 $x$ 坐标。相对误差可以在 $10^{-4}$ 之内。你可以假设存在唯一解决方案。没有数据会导致竖井距离 qanat 渠道出口或其他竖井小于0.001单位。

### **说明/提示**

时间限制：$2000$ ms，空间限制：$1048576$ kB。

来源：

> International Collegiate Programming Contest (ACM-ICPC) World Finals 2015

```input1
8 4 1

```

```output1
31.500000
3.000000

```

```input2
195 65 2

```

```output2
12220.000000
48.000000
108.000000

```

```input3
10000 1 1000

```

```output3
30141.885677
9.956721
19.913443
29.870164
39.826887
49.783610
59.740334
69.697060
79.653786
89.610515
99.567245

```

## 提示
Time limit: 2000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2015


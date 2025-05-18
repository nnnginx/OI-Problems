## 题目背景
本题译自 [Canadian Computing Competition](https://cemc.uwaterloo.ca/resources/past-contests?contest_category=29) [2020 Junior](https://cemc.uwaterloo.ca/sites/default/files/documents/2020/2020CCCJrProblemSet.html) T3 Art。

## 题目描述
Mahima 一直在尝试一种新的艺术风格。她站在画布前，用画笔在画布上绘画。当她认为自己创造了一件杰作时，她会用3D打印机打印一个框架来保护自己的画作。

你的工作是通过确定尽可能小的长方形框架的坐标来帮助 Mahima，让每一滴颜料都位于框架内。

**框架上的点不在框架内考虑。**

## 输入格式
第一行一行一个整数 $n(2\le n \le100)$ 表示颜料的数量。

接下来 $n$ 行每行两个整数 $x,y(x,y \le 100)$，表示当前颜料的坐标，中间用 `,` 分割。

## 输出格式
共两行。

第一行两个整数表示框架左上角的坐标，用 `,` 分割。

第二行两个整数表示框架右下角的坐标，用 `,` 分割。

```input1
5
44,62
34,69
24,78
42,44
64,10
```

```output1
23,9
65,79
```

## 提示
**本题采用捆绑测试**。
#### 【样例解释】
框架的左下角是 $(23,9)$，如果左下角上移，则颜料 $(64,10)$ 将不再位于框架内，如果其右移，则颜料 $(24,78)$ 将不再位于框架，而向其他方向移动会加大框架面积，不合题意。右上角同理。
![](https://cdn.luogu.com.cn/upload/image_hosting/qrrjbsb8.png)


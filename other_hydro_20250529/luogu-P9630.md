## 题目描述
Kotori is interested in skiing. The skiing field is an infinite strip going along $y$-axis on the 2-dimensional plane where all points $(x, y)$ in the field satisfies $-m \le x \le m$. When skiing, Kotori cannot move out of the field, which means that the absolute value of his $x$-coordinate should always be no more than $m$. There are also $n$ segments on the ground which are the obstacles and Kotori cannot move across the obstacles either.

Kotori will start skiing from $(0, -10^{10^{10^{10^{10}}}})$ (you can regard this $y$-coordinate as a negative infinity) and moves towards the positive direction of the $y$-axis. Her vertical (parallel to the $y$-axis) speed is always $v_y$ which cannot be changed, however she can control her horizontal (parallel to the $x$-axis) speed in the interval of $[-v_x, v_x]$. The time that Kotori changes her velocity can be neglected.

Your task is to help Kotori calculate the minimum value of $v_x^*$ that once $v_x>v_x^*$ she can safely ski through the skiing field without running into the obstacles.

## 输入格式
There is only one test case in each test file.

The first line of the input contains three positive integers $n$, $m$ and $v_y$ ($1 \le n \le 100$, $1 \le m \le 10^4$, $1 \le v_y \le 10$), indicating the number of obstacles, the half width of the skiing field and the vertical speed.

For the following $n$ lines, the $i$-th line contains four integers $x_1$, $y_1$, $x_2$ and $y_2$ ($-m \le x_1, x_2 \le m$, $-10^4 \le y_1, y_2 \le 10^4$, $x_1 \ne x_2$ or $y_1 \ne y_2$) indicating the $i$-th obstacle which is a segment connecting point $(x_1, y_1)$ and $(x_2, y_2)$, both inclusive (that is to say, these two points are also parts of the obstacle and cannot be touched). It's guaranteed that no two obstacles intersect with each other.

## 输出格式
Output one line containing one number indicating the minimum value of $v_x^*$. If it is impossible for Kotori to pass through the skiing field, output ``-1`` (without quotes) instead.

Your answer will be considered correct if and only if its absolute or relative error does not exceed $10^{-6}$.

## 题目大意
### 题目描述
Kotori 对滑雪很感兴趣。滑雪场是在二维平面上沿着 $y$ 轴无限延伸的直线，其中场中的所有点 $(x,y)$ 满足 $-m\le x\le m$。滑雪时，Kotori 不能离开场地，这意味着他的 $x$ 坐标的绝对值应该始终不超过 $m$。地面上也有 $n$ 个路段是障碍，Kotori 无法越过障碍。

Kotori 将从 $(0, -10^{10^{10^{10^{10}}}})$  开始滑雪（你可以将此 $y$ 坐标视为负无穷大），并朝着 $y$ 轴的正方向移动。她的垂直（平行于 $y$ 轴）速度始终是 $v_y$，此值不变，但是她可以在 $[-v_x, v_x]$ 的间隔内控制她的水平（平行于 $x$ 轴的）速度。Kotori 改变速度的时间可以忽略不计。

你的任务是帮助 Kotori 计算 $v_x^*$ 的最小值，即一旦 $v_x>v_x^*$，她就可以安全地穿过滑雪场而不会遇到障碍物。

### 输入格式

每个测试文件中只有一个测试用例。

输入的第一行包含三个正整数 $n, m$ 和 $v_y$（$1\le n\le 100$，$1\le m\le 10^4$，$1\le v_y\le 10$），分别表示障碍物的数量、滑雪场的半宽和垂直速度。

对于下面的 $n$ 行，第 $i$ 行包含四个整数 $x_1, y_1, x_2$ 和 $y_2$（$-m\le x_1, x_2\le m$，$-10^4\le y_1, y_2\le 10^4$，$x_1\ne x_2$ 或 $y_1\ne y_2$），这四个整数表示第 $i$ 个障碍物，该障碍物是连接点 $(x_1, y_1)$ 和 $(x_2, y_2)$ 的线段，两者都包括在内（也就是说，这两个点也是障碍物的一部分，不能触摸）。保证没有两个障碍物相互交叉。

### 输出格式

输出一行，其中包含一个数字，表示 $v_x^*$ 的最小值。如果 Kotori 无法通过滑雪场，请输出 `-1`（不带引号）。

当且仅当其绝对或相对误差不超过 $10^{-6}$ 时，您的答案才会被认为是正确的。

------------

翻译来自 [fire_wolf](https://www.luogu.com.cn/user/690669)。

```input1
3 2 1
-2 0 1 0
-1 4 2 4
0 1 0 3
```

```output1
1.000000000000000
```

```input2
2 1 2
-1 0 1 0
1 1 0 1
```

```output2
-1
```

```input3
2 3 7
-3 0 2 2
3 1 -2 17
```

```output3
1.866666666666666
```

```input4
1 100 1
-100 0 99 0

```

```output4
0.000000000000000
```


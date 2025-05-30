## 题目描述
You are the God of Wind.

By moving a big cloud around, you can decide the weather: it invariably rains under the cloud, and the sun shines everywhere else.

But you are a benign God: your goal is to give enough rain to every field in the countryside, and sun to markets and festivals. Small humans, in their poor vocabulary, only describe this as "weather forecast".

You are in charge of a small country, called Paccimc. This country is constituted of 4 x 4 square areas, denoted by their numbers.

![](https://cdn.luogu.com.cn/upload/image_hosting/tuq65kcj.png)

Your cloud is of size 2 x 2, and may not cross the borders of the country.

You are given the schedule of markets and festivals in each area for a period of time.

On the first day of the period, it is raining in the central areas (6-7-10-11), independently of the schedule.

On each of the following days, you may move your cloud by 1 or 2 squares in one of the four cardinal directions (North, West, South, and East), or leave it in the same position. Diagonal moves are not allowed. All moves occur at the beginning of the day.

You should not leave an area without rain for a full week (that is, you are allowed at most 6 consecutive days without rain). You don't have to care about rain on days outside the period you were given: i.e. you can assume it rains on the whole country the day before the period, and the day after it finishes.


## 输入格式
The input is a sequence of data sets, followed by a terminating line containing only a zero.

A data set gives the number N of days (no more than 365) in the period on a single line, followed by N lines giving the schedule for markets and festivals. The i-th line gives the schedule for the i-th day. It is composed of 16 numbers, either 0 or 1, 0 standing for a normal day, and 1 a market or festival day. The numbers are separated by one or more spaces.

## 输出格式
The answer is a 0 or 1 on a single line for each data set, 1 if you can satisfy everybody, 0 if there is no way to do it.

## 题目大意
**【题目描述】**

你是风之神。

通过移动一朵大云，你可以决定天气：云下必定下雨，其他地方阳光普照。

但你是一个仁慈的神：你的目标是给乡间的每个田地带来足够的雨水，给市场和节日带来阳光。小人类用他们贫乏的词汇，只能将这称为“天气预报”。

你负责管理一个名为 Paccimc 的小国家。这个国家由 $4 \times 4$ 的方块区域组成，用它们的编号表示。

![](https://cdn.luogu.com.cn/upload/image_hosting/tuq65kcj.png)

你的云的大小为 $2 \times 2$，不得越过国家的边界。

给出了一段时间内每个区域的市场和节日的安排。

在该时段的第一天，无论安排如何，在中心区域（6-7-10-11）都会下雨。

在接下来的每一天，你可以将你的云向四个基本方向之一（北、西、南和东）移动 $1$ 或 $2$ 个方格，也可以将其保持在原位。不允许对角线移动。所有移动均发生在一天开始时。

你不应该让一个区域连续一周没有雨水（也就是说，你允许最多连续 $6$ 天没有雨）。你不必在你获得的时间段之外的日子里考虑雨水：也就是说，你可以假设在时间段之前的整个国家都下雨，在它结束后的一天也是如此。

**【输入格式】**

输入一个数据集序列，后跟一个仅包含零的终止行。

一个数据集在单独的一行上给出了期间中的天数 $N$（不超过 $365$），然后是 $N$ 行，给出了市场和节日的安排。第 $i$ 行给出了第 $i$ 天的安排。它由 $16$ 个数字组成，要么是 $0$ 要么是 $1$，$0$ 表示正常日，$1$ 表示市场或节日。数字之间用一个或多个空格分隔。

**【输出格式】**

对每个数据集的单行输出，如果你能满足每个人，则输出 $1$，否则输出 $0$。

**【样例解释】**

翻译来自于：[ChatGPT](https://chatgpt.com/)

```input1
1 
0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 
7
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
1 0 0 0 0 0 1 0 0 0 0 1 1 0 0 1 
0 0 0 0 0 0 0 0 1 0 0 0 0 1 0 1 
0 0 0 0 0 0 0 0 0 1 0 1 0 0 0 0 
0 1 0 1 0 0 0 0 0 0 0 0 0 0 0 0 
1 0 0 1 0 0 0 0 0 0 0 0 0 0 0 1 
0 0 0 0 0 1 0 0 1 0 0 0 0 0 0 0 
7 
0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 
0 0 1 0 0 0 0 1 0 0 0 0 0 1 0 0 
0 0 0 1 0 0 0 0 0 0 1 0 1 0 0 0 
0 1 0 0 0 0 0 1 0 0 0 0 1 0 0 0 
0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 1 1 0 1 0 0 0 0 1 
0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0
15 
0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 
0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 1 1 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0  
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0  
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 1 1 0 1 0 0 0 0 
0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 
0 0 1 1 0 0 0 0 0 1 0 0 0 0 0 0 
1 1 0 0 0 0 0 0 0 0 1 0 0 1 0 0 
0 0 0 0 0 1 0 0 0 0 0 1 0 0 0 0  
0 0 1 0 0 0 0 0 0 0 0 0 0 0 1 0 
1 0 0 1 1 0 0 0 0 1 0 1 0 0 0 0 
0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 
0 0 0 0 0 1 0 1 0 1 0 0 0 0 0 0  
0
```

```output1
0
1
0
1
```


## 题目描述
![](https://cdn.luogu.com.cn/upload/image_hosting/jnez9lpt.png)

Images by John Fowler, Carol Highsmith, and Richard Woodland

You have decided to spend a day of your trip to Rapid City taking photographs of the South Dakota Badlands, which are renowned for their spectacular and unusual land formations. You are an amateur photographer, yet very particular about lighting conditions.

After some careful research, you have located a beautiful location in the Badlands, surrounded by picturesque landscapes. You have determined a variety of features that you wish to photograph from this location. For each feature you have identified the earliest and latest time of day at which the position of the sun is ideal. However, it will take quite a bit of time to take each photograph, given the need to reposition the tripod and camera and your general perfectionism. So you are wondering if it will be possible to successfully take photographs of all these features in one day.



## 输入格式


The first line of the input contains two integers $n (1 \le n \le 10^{4})$ and $t (1 \le t \le 10^{5}),$ where $n$ is the number of desired photographs and $t$ is the time you spend to take each photograph. Following that are $n$ additional lines, each describing the available time period for one of the photographs. Each such line contains two nonnegative integers a and $b$ , where a is the earliest time that you may begin working on that photograph, and $b$ is the time by which the photograph must be completed, with a $+ t \le b \le 10^{9}.$



## 输出格式


Display yes if it is possible to take all $n$ photographs, and no otherwise.



## 题目大意
你要拍 $n$ 张照片，每张照片必须在 $[a_i,b_i]$ 这个时间段内完成拍摄，并且拍每一张图片都需要用 $t$ 的时间，同一个时间内只能拍摄一张图片。求是否能拍摄完所有照片。

$1 \le n \le 10^4$，$1 \le t \le 10^5$，$a_i+t \le b_i \le 10^9$。

翻译者：一只书虫仔

```input1
2 10
0 15
5 20

```

```output1
yes

```

```input2
2 10
1 15
0 20

```

```output2
no

```

```input3
2 10
5 30
10 20

```

```output3
yes

```

## 提示
Time limit: 6 s, Memory limit: 512 MB. 




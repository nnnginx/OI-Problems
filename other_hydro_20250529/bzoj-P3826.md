[](/d/bzoj/p/3893)

## 题目描述
Farmer John's N cows (1 <= N <= 100,000) are out exercising their hooves again, jogging along an infinite track.  Each cow starts at a distinct position on the track, and some cows run at different speeds. The track is divided into lanes so that cows may move past each other. No two cows in the same lane may ever occupy the same position. Farmer John doesn't want any cow to have to change lanes or adjust speed, and he wonders how many lanes he will need to accomplish this if the cows are going to run for T minutes (1 <= T <= 1,000,000,000).
给出N头牛，每头牛有自己的初始位置及奔跑的速度。它们要跑T分钟，现在不希望他们的跑的过程中出现“撞车”即跑到同一个点上，因而要将道路分成若干个跑道，问至少要多少个跑道。
## 输入格式
The first line of input contains N and T. The following N lines each contain the initial position and speed of a single cow.  Position is a nonnegative integer and speed is a positive integer; both numbers are at most 1 billion.  All cows start at distinct positions, and these will be given in increasing order in the input.
## 输出格式
A single integer indicating the minimum number of lanes necessary so that no two cows in the same lane ever occupy the same location (including at time T).

```input1
5 3
0 1
1 2
2 3
3 2
6 1

```

```output1
3
```

## 提示
没有写明提示
## 题目来源
没有写明来源



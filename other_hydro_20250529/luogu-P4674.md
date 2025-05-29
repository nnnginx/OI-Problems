## 题目描述
A company of $n$ employees is due for a restructuring. In the resulting hierarchy,represented as a rooted tree, every node will be the boss of its children.

Each employee has a list of bosses they will accept. In addition, all employees mustbe assigned a salary. The salary must be a positive integer, and the salary of eachboss must be larger than the sum of salaries of their immediate subordinates.

Your task is to structure the company so that all above conditions hold, and the sumof all the salaries is as small as possible.

## 输入格式
The first input line contains an integer $n$ : the number of employees. The employees are numbered $1,2,...,n$

.After this, the input contains $n$ lines that describe the preferences of the employees.The $i$th such line contains an integer $k_i$ , followed by a list of $k_i$ integers. The list consists of all employees that the $i$th employee accepts as their boss.

## 输出格式
You should output the lowest total salary among all valid restructurings. You can assume that at least one solution exists.

## 题目大意
[BalticOI 2016 Day1]上司们

## 题目描述

一家有 $n$ 名员工的公司将进行重组。在重组后的层级结构中（表示为一棵有根树），每个节点将作为其子节点的上司。

每位员工都有一个可以接受的上司列表。此外，所有员工都必须被分配一个薪水。薪水必须是一个正整数，并且每位上司的薪水必须大于其直接下属薪水之和。

你的任务是安排公司的结构，以确保满足上述所有条件，并且所有员工的薪水总和尽可能小。

## 输入格式

第一行输入包含一个整数 $n$ ，表示员工数量。员工编号为 $1, 2, \dots, n$。

接下来的 $n$ 行描述每个员工的上司偏好。第 $i$ 行包含一个整数 $k_i$，后跟一个 $k_i$ 整数的列表。该列表包括第 $i$ 位员工可以接受的所有上司的编号。

## 输出格式

你需要输出所有符合条件的重组方案中，最低的薪水总和。可以假设至少存在一种可行方案。

```input1
4
1 4
3 1 3 4
2 1 2
1 3

```

```output1
8
```

## 提示
### Subtask 1 (22 points)

- $2\leq n \leq 10$

- $\sum^n_{i=1}k_i\leq 20$

### Subtask 2 (45 points)

- $2\leq n \leq 100$

- $\sum^n_{i=1}k_i\leq 200$

### Subtask 3 (33 points)

- $2\leq n \leq 5000$

- $\sum^n_{i=1}k_i\leq 10000$


## 题目描述


Election committee of Flatland is preparing for presidential elections. To minimize human factor in ballot counting they decided to develop an automated Ballot Analyzing Device $(BAD).$

There are $n$ candidates running for president. The ballot contains one square field for each candidate. The voter must mark exactly one of the fields. If no field is marked or there are two or more marked fields, the ballot is invalid. Each voter puts $his/her$ ballot to a special scanner in BAD. The scanner analyzes marks on the ballot and creates a special voting string of $n$ characters: $‘X'$ for marked field and $‘. '$ for unmarked one. Now voting strings must be analyzed to get the report. Your task is to develop a report generator for BAD.

Given voting strings for all ballots, your program must print the voting report. Candidates in the report must be arranged in order of decreasing number of votes. If two candidates have the same number of votes, they must have the same order as in a voting ballot. For each candidate calculate $his/her$ result in percent (if the candidate received $p$ votes, the result in percent is $100p/m)$ . The last line of the report must indicate the percentage of the invalid ballots.



## 输入格式


The first line contains two integers $n$ and $m$ -- the number of candidates and the number of ballots $(2 \le n \le 10$ ; $1 \le m \le 1000)$ . The following $n$ lines contain last names of candidates. Each name is a string of at most $100$ English letters. There is no candidate named `Invalid`.

Then $m$ lines follow, each of them contains one voting string.



## 输出格式


Print n+ $1$ lines. First print results for candidates in percent. For each candidate print $his/her$ last name followed by a space and then $his/her$ result in percent and a percent sign $‘\%'.$ The last line must specify the percentage of invalid ballots: a word `Invalid` followed by a space, the percentage of invalid ballots and a percent sign.

Round all numbers to exactly two digits after the decimal point. If the number is exactly in the middle of two representable numbers, output the greater one (e.g . output `12 . $35`$ for $12$ . $345$) .



## 题目大意
有 $n$ 名选手参加一个比赛，有 $m$ 个人为他们投票。第 $i$ 个人的投票情况用一个长度为 $n$，并且仅包含 `.` 和 `X` 两个字符的字符串，其中，如果第 $j$ 位是 `X`，则第 $i$ 个人将票投给了第 $j$ 名选手，否则没有。规定每个投票者能且仅能将票投给一个人，否则都算无效票（即投的票数 $\geqslant 2$ 或者 $=0$）。请将每名选手按照他们所得到的票的比例排序（如果有两名选手得到的票的比例相同，在投票次序中先出现的那名选手排在前面），并输出他们的名字和得票比例，最后还要输出无效票所占的比例。

Translated by Eason_AC  
2020.11.12

```input1
4 7
Loudy
Apples
Dogman
Miller
.X..
X...
....
..X.
..XX
..X.
..X.

```

```output1
Dogman 42.86%
Loudy 14.29%
Apples 14.29%
Miller 0.00%
Invalid 28.57%

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 




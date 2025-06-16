# AT_code_festival_2015_okinawa_d Dictionary for Shiritori Game

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2015-okinawa-open/tasks/code_festival_2015_okinawa_d

## 输入格式

Inputs will be given by standard input in following format.

> $ N $ $ M $ $ p_1 $ $ q_1 $ $ p_2 $ $ q_2 $ : $ p_M $ $ q_M $

- At the first line, an integer $ N(1≦N≦100,000) $、$ M(1≦M≦200,000) $ will be given.
- From the second line there are $ M $ lines that represent all the words in this dictionary. For the $ i_{th} $ line, integer $ p_i(1≦p_i≦N) $ and $ q_i(1≦q_i≦N) $ will be given divided by space.

It is possible that there are different words that begin with the same character and end with the same character. In other words, it is possible that $ p_i\ =\ p_j $ and $ q_i\ =\ q_j $ even when $ i\ \neq\ j $.

## 输出格式

Assume that two players will try their best. Output `Snuke` if the first player wins, output `Sothe` if the second player wins in one line. If the game will never halt, output `Draw` in one line.

Print a newline at the end of output.

## 输入输出样例 #1

### 输入 #1

```
6 5
1 2
2 3
3 4
4 2
2 5
```

### 输出 #1

```
Sothe
```

## 输入输出样例 #2

### 输入 #2

```
6 6
1 2
2 3
3 4
4 2
2 5
5 6
```

### 输出 #2

```
Draw
```

## 输入输出样例 #3

### 输入 #3

```
6 8
1 2
1 3
3 4
3 5
2 1
4 5
4 6
5 6
```

### 输出 #3

```
Snuke
```

## 输入输出样例 #4

### 输入 #4

```
4 8
2 3
2 3
3 4
4 1
3 1
2 2
4 2
4 3
```

### 输出 #4

```
Sothe
```

## 说明/提示

### Problem

In a country where $ N $ different kinds characters are being used, there is a dictionary that contains $ M $ entries, each entry is a definition for a word. All the kinds of characters are listed as character $ 1 $, character $ 2 $, ..., character $ N $. The $ i_{th} $ entry (as a word) of this dictionary begins with the letter $ p_i $, and ends with the letter $ q_i $.

 Cat Snuke and Wolf Sothe will use this dictionary to play a game called **Shiritori** . (Please note that Shiritori in this game is different from a normal Shiritori game.)

- The first move will be made by Cat Snuke, then two players will move alternately.
- For the first move, the player in turn has to say a word the begins with character $ 1 $. If there are no any words that begin with character $ 1 $, the player in turn loses.
- For the rest moves, the player of that turn has to say any word that begins with the last character of the word being said in the previous move from the dictionary. If there is not any appropriate word, the player in turn loses.
- **Any word can be said any number of times** .

There should be some dictionaries that two players can not change the result of the game even if they tried their best. For these dictionaries, in this case, we want to find out if the first player or the second player will win, or even the game will never halt.

All the words in the dictionary will be given. We can assume that the two players will try their best. Please decide if the first player (Cat Snuke) or the second player (Wolf Sothe) will win, or even the game will never halt.

### Sample Explanation 1

\- For the first move, Cat Snuke has to say the first word. - For the second move, if Wolf Sothe said the 6th word, Cat Snuke will have no appropriate word to say for the next move, thus Wolf Sothe wins.

### Sample Explanation 4

Please note that for the first move it is possible that there is no appropriate word that can be said.
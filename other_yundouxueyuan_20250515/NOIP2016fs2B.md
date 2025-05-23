# Description

本题中,我们将用符号 [ *c* 」表示对 *c* 向下取整,例如: [3.0」= [3. 1」= [3.9」= 3 。

蛐蛐国最近蚯蚓成灾了!隔壁跳蚤国的跳蚤也拿蚯蚓们没办法,蛐蛐国王只好去 请神刀手来帮他们消灭蚯蚓。

蛐蛐国里现在共有*n* 只蚯蚓 ( *n* 为正整数）。每只蚯蚓拥有长度,我们设第 *i* 只蚯 蚓的长度为$a_i$  ( *i* = 1, 2, . . . , *n* ) ,并保证所有的长度都是非负整数 (即:可能存在长度为 0 的蚯蚓）。

每一秒,神刀手会在所有的蚯蚓中,准确地找到最长的那一只 (如有多个则任选 一个）将其切成两半。神刀手切开蚯蚓的位置由常数*p*   (是满足 0 < *p* < 1 的有理数） 决定,设这只蚯蚓长度为*x* ,神刀手会将其切成两只长度分别为 [*p* *x* 」和 *x* - [*p* *x* 」的蚯 蚓。特殊地,如果这两个数的其中一个等于 0 ,则这个长度为 0 的蚯蚓也会被保留。此 外,除了刚刚产生的两只新蚯蚓,其余蚯蚓的长度都会增加*q*   (是一个非负整常数）。

蛐蛐国王知道这样不是长久之计,因为蚯蚓不仅会越来越多,还会越来越长。蛐 蛐国王决定求助于一位有着洪荒之力的神秘人物,但是救兵还需要 *m* 秒才能到来. . . . . . ( *m* 为非负整数）

蛐蛐国王希望知道这 *m* 秒内的战况。具体来说,他希望知道:

●  *m* 秒内,每一秒被切断的蚯蚓被切断前的长度 (有 *m* 个数）:

●  *m* 秒后,所有蚯蚓的长度 (有 *n* + *m* 个数）。

蛐蛐国王当然知道怎么做啦!但是他想考考你. . . . . .

# Format

## Input

从文件***ea******rt******h******w******o******r******m***  ***.*** ***i******n*** 中读入数据。

第一行包含六个整数  *n* ,  *m* ,  *q* ,  *u* ,  *v* , *t* ,其中:  *n* ,  *m* , *q* 的意义见【问题描述】:  *u* ,  *v* , *t* 均 为正整数:你需要自己计算*p* =  *u* /*v*   (保证 0 < *u* < *v* ）: *t* 是输出参数,其含义将会在 【输出格式】中解释。

第二行包含 *n* 个非负整数,为 $a_1$ , $a_2$ , . . . , $a_n$,即初始时*n* 只蚯蚓的长度。 同一行中相邻的两个数之间,恰好用一个空格隔开。

保证 1 s *n* s 105  , 0 s *m* s 7 x 106  , 0 < *u* < *v* s 109  , 0 s *q* s 200 , 1 s *t* s 71 , 0 s $a_i$  s 108  。

## Output

输出到文件***ea******rt******h******w******o******r******m***  ***.*** ***o******u******t*** 中。
第一行输出'$\frac mt$'个整数,按时间顺序,依次输出第 *t* 秒,第 2*t* 秒,第 3*t* 秒,. . . . . . 被 切断蚯蚓 (在被切断前）的长度。
第二行输出'$\frac {n+m}{t}$'个整数,输出*m* 秒后蚯蚓的长度:需要按从大到小的顺序,依 次输出排名第 *t* ,第 2*t* ,第 3*t* ,. . . . . . 的长度。
同一行中相邻的两个数之间,恰好用一个空格隔开。 即使某一行没有任何数需要 输出,你也应输出一个空行。
请阅读样例来更好地理解这个格式。

# Samples

```input1
3  7  1  1  3  1
3  3  2
```

```output1
3  4  4  4  5  5  6
6  6  6  5  5  4  4  3  2  2
```

```input2
3  7  1  1  3  2
3  3  2
```

```output2
4  4  5
6  5  4  3  2
```

```input3
3  7  1  1  3  9
3  3  2
```

```output3
2
```



# Limitation

【样例1说明】
在神刀手到来前:3只蚯蚓的长度为3,3,2。
1秒后:一只长度为3的蚯蚓被切成了两只长度分别为1和2的蚯蚓,其余蚯蚓的长 度增加了1。最终4只蚯蚓的长度分别为(1,2),4,3。括号表示这个位置刚刚有一只蚯蚓被 切断。
2秒后:一只长度为4的蚯蚓被切成了1和3。5只蚯蚓的长度分别为:2,3,(1,3),4。  3秒后:一只长度为4的蚯蚓被切断。6只蚯蚓的长度分别为:3,4,2,4,(1,3)。       4秒后:一只长度为4的蚯蚓被切断。7只蚯蚓的长度分别为:4,(1,3),3,5,2,4。     5秒后:一只长度为5的蚯蚓被切断。8只蚯蚓的长度分别为:5,2,4,4,(1,4),3,5。   6秒后:一只长度为5的蚯蚓被切断。9只蚯蚓的长度分别为:(1,4),3,5,5,2,5,4,6。  7秒后:一只长度为6的蚯蚓被切断。 10只蚯蚓的长度分别为:2,5,4,6,6,3,6,5,(2,4)。
所以,7秒内被切断的蚯蚓的长度依次为3,4,4,4,5,5,6。7秒后,所有蚯蚓长度从大 到小排序为6,6,6,5,5,4,4,3,2,2。

【样例2说明】
这个数据中只有*t* = 2 与上个数据不同。 只需在每行都改为每两个数输出一个数即 可。
虽然第一行最后有一个6没有被输出,但是第二行仍然要重新从第二个数再开始输 出。

【样例3说明】
这个数据中只有*t* = 9 与上个数据不同。
注意第一行没有数要输出,但也要输出一个空行。

【子任务】
● 测试点1 ~ 3 满足*m* = 0 。
● 测试点4 ~ 7 满足  *n* , *m* s 1, 000 。
● 测试点8 ~ 14 满足*q* = 0 ,其中测试点 8 ~ 9 还满足*m* s 105  。
● 测试点15 ~ 18 满足 *m* s 3 x 105  。
● 测试点19 ~ 20 没有特殊的约定,参见原始的数据范围。
● 测试点1 ~  12 , 15 ~  16 还满足 *v*  s  2 ,这意味着  *u* , *v* 的唯一可能的取值是
*u* = 1, *v* = 2 ,即 *p* = 0.5 。这可能会对解决问题有特殊的帮助。 每个测试点的详细数据范围见下表。

| 测试点 | *n*       | *m* |   | *t*     | *a**i*     | *v*        | *q*   |
| -------- | ------------ | ------ | --- | ---------- | -------------- | ------------- | -------- |
| 1      | = 1        |  = 0 |   |      = 1 |        s 106 |         s 2 |    = 0 |
| 2      | = 103      |
| 3      | = 105      |
| 4      | = 1        |   = 103 |   |
| 5      | = 103      |
| 6      | = 1        | s 200 |
| 7      | = 103      |
| 8      | = 5 x 104  | = 5 x 104 |   |     = 0 |
| 9      |            | = 105 |   | = 2 |
| 10     |            | = 2 x 106 |   | = 21 |
| 11     | = 105      | =2.5x 106 |   | = 26 |
| 12     | =3.5x 106  |   | = 36 | s 107 |
| 13     |            | = 5 x 106 |   | = 51 | s 109 |
| 14     |            | = 7 x 106 |   | = 71 |     s 108 |
| 15     | = 5 x 104  | = 5 x 104 |   | = 1 | s 2 |     s 200 |
| 16     | = 1 5 x105 |   | = 2 |
| 17     |            | = 105 |   | = 3 |   s 109 |
| 18     | = 105      | = 3 x 105 |   | =4 |
| 19     | =3.5x 106  |   | = 36 |
| 20     |            | = 7 x 106 |   | = 71 |


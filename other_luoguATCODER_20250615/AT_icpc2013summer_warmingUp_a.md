# AT_icpc2013summer_warmingUp_a Anime Master

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2013summer-warmingup/tasks/icpc2013summer_warmingUp_a

KM really likes Anime (Japanese animation).  
 He is trying to watch as many animes as possible.  
 The anime is broadcast at the same time zone every week.  
 Because he is a perfectionist, he must watch the same animes every week.  
 Moreover he can't watch animes which are broadcast at the same time or watch them later by recording them.  
 KM is a really excellent mathematician but because a lot of animes are broadcast, he couldn't find the best solution for this problem.  
 Can you, the excellent programmer, solve this problem?  
 The first line of the input file contains $ N $ and $ M $ ($ 1\ \leq\ N\ \leq\ 10^5 $, $ 2\ \leq\ M\ \leq\ 10^6 $), which is the number of animes and the length of a week, respectively.  
 In KM's country, the week is composed of $ M $ unit time.  
 Each of the following $ N $ lines gives start time $ s $ and end time $ t $ of each animes. ($ 0\ \leq\ s,\ t\ ,\ s\ \neq\ t $)  
 $ s\ >\ t $ means the anime lasts over the boundary of the week.  
 It is possible to watch two animes whose end time is same as the other's start time.  
 Output the maximal number of animes he can watch.

```

3 10
0 3
3 7
7 0
```

 ```

3
```

 ```

3 10
0 5
2 7
6 9
```

 ```

2
```

 ```

5 10
1 6
2 7
3 8
4 9
5 0
```

 ```

1
```

## 输入格式

无

## 输出格式

无
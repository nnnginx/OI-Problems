## Description

<div><p>A movie company has released $2$ movies. These $2$ movies were watched by $n$ people. For each person, we know their attitude towards the first movie (liked it, neutral, or disliked it) and towards the second movie.</p><p>If a person is asked to leave a review for the movie, then: </p><ul> <li> if that person liked the movie, they will leave a positive review, and the movie's rating will increase by $1$; </li><li> if that person disliked the movie, they will leave a negative review, and the movie's rating will decrease by $1$; </li><li> otherwise, they will leave a neutral review, and the movie's rating will not change. </li></ul><p>Every person will review exactly one movie ！ and for every person, you can choose which movie they will review.</p><p>The company's rating is the minimum of the ratings of the two movies. Your task is to calculate the maximum possible rating of the company.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-1 \le a_i \le 1$), where $a_i$ is equal to $-1$ if the first movie was disliked by the $i$-th viewer; equal to $1$ if the first movie was liked; and $0$ if the attitude is neutral.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($-1 \le b_i \le 1$), where $b_i$ is equal to $-1$ if the second movie was disliked by the $i$-th viewer; equal to $1$ if the second movie was liked; and $0$ if the attitude is neutral.</p><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the maximum possible rating of the company, if for each person, choose which movie to leave a review on.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-1 \le a_i \le 1$), where $a_i$ is equal to $-1$ if the first movie was disliked by the $i$-th viewer; equal to $1$ if the first movie was liked; and $0$ if the attitude is neutral.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($-1 \le b_i \le 1$), where $b_i$ is equal to $-1$ if the second movie was disliked by the $i$-th viewer; equal to $1$ if the second movie was liked; and $0$ if the attitude is neutral.</p><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the maximum possible rating of the company, if for each person, choose which movie to leave a review on.</p>





```input1|2,3,4,8,9,10
4
2
-1 1
-1 -1
1
-1
-1
5
0 -1 1 0 1
-1 1 0 0 1
4
-1 -1 -1 1
-1 1 1 1
```




```output1
0
-1
1
1
```



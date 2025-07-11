## 题目描述
In the world of rising AI, James is scared of losing his job. So, when his boss asks him to evaluate a new AI model to see how well it performs compared to humans, he wants to make it look as bad as possible.

To test the AI, James conducts a sequence of $N$ trials where a human and an AI are
given the same task and then scored based on their performance on the task. 
He is then going to send the results of some non-empty contiguous subsequence of these trials to his boss and quietly delete the rest.

Let $a_i$ and $h_i$ be the performance of the AI and human on trial $i$, respectively. James's boss evaluates the AI on a sequence of trials by calculating two total scores: one for the humans, and one for the AI. Both scores are initially $0$. For each trial $i$ where $h_i \geq a_i$, the boss awards the humans $h_i-a_i$ points. For each trial where $h_i < a_i$, the AI earns $a_i-h_i$ points.
If the humans' total score is greater than or equal to the AI's total score times some constant $k$ (to account for humans needing food, water, and a desk), James's boss declares that the humans outperform the AI.

James plans to send his chosen subsequence of test results through email to his boss. There is, however, one complication: since AI is already all-knowing and all-pervasive, it intercepts this email and may swap the value of $h_i$ and $a_i$ for one trial $i$ of its choice. (It doesn't want to swap more than one trial result---James might notice!)

Count how many non-empty contiguous subsequences of trial results James could send his boss with the guarantee that humans will be declared to outperform the AI, even if the AI swaps the result of up to one trial.

## 输入格式
The first line of input contains two space-separate integers: $N$ ($1 \leq N \leq 2 \cdot 10^5$), the total number of trials James conducted, and $k$ ($1 \leq k \leq 100$), the multiplier James's boss will apply to the AI's total score to determine whether humans outperform AI.

The second line contains $N$ space-separated integers $h_1, h_2, \ldots, h_N$ ($0 \leq h_i \leq 10^6$), the performance of the humans on each of the $N$ trials.

The third line contains $N$ space-separated integers $a_1, a_2, \ldots, a_N$ ($0 \leq a_i \leq 10^6$), the performance of the AI on the $N$ trials.

## 输出格式
Print the number of non-empty contiguous trial subsequences for which James's boss would declare that humans outperform AI, even if the AI swaps the result of up to one trial.

```input1
10 2
3 5 7 6 8 6 4 5 2 6
2 4 6 5 4 3 3 6 3 4
```

```output1
4
```

```input2
7 1
4 3 2 1 7 6 5
4 2 3 1 7 6 5
```

```output2
11
```


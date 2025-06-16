## 题目描述
King Primonidas is putting together a tournament to find the strongest gladiator in all the lands. In total $N$ gladiators have made their way to the Coliseum to bring back honor and glory to their hometowns. Each gladiator starts with a certain amount of vitality. Vitality is similar to health points in that it reflects the amount of damage a gladiator can take, but it also represents the amount of damage they can deal (since energy is needed for strong blows).

The tournament consists of $K$ rounds. Every round, the king arranges the gladiators in a line from least to most remaining vitality, breaking ties randomly. King Primonidas believes that the true strength of a gladiator lies in their ability to take a beating, so he orders the first gladiator (the one with the lowest remaining vitality) to deal their strongest blow to the second gladiator. This blow subtracts the first gladiator's vitality from the second gladiator's vitality. After the second gladiator takes the hit, they deal their strongest blow (using their new, lowered vitality) to the third gladiator, and so on. This process repeats until the second-to-last gladiator deals their strongest blow to the last gladiator (who doesn't get to attack anybody).

Notice that in the above process, a gladiator's vitality can never go below zero. (A gladiator with zero vitality deals a feeble blow of no damage to the next gladiator.)

Print the vitality of each gladiator after $K$ tournament rounds, in order from the first to the last gladiator in line.

## 输入格式
The first line of input contains two space-separated integers $N$ ($2 \leq N \leq 10^5$) and $K$ ($1 \leq K \leq 10^{18}$): the number of gladiators and the number of rounds in the tournament.

The next line of input contains $N$ space-separated integers $v_1 \; v_2 \; \ldots v_N$ ($0 \leq v_i \leq 10^{18}$): the starting vitality of the gladiators.

## 输出格式
Print $N$ space-separated integers: the vitality of the gladiators at the end of the $K$th round of the tournament, in the order that the gladiators currently stand in line.

```input1
6 3
21 28 24 23 1 12
```

```output1
1 1 3 6 3 10

```

```input2
3 1000
8 2 10

```

```output2
0 0 2
```


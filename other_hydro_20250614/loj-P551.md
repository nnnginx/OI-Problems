## Description


Alex is playing a game with Ball. There is a blank matrix $M$ with $n$ lines and $n$ columns. Alex and Ball take turns to mark one of the matrix elements with his own sign (Alex¡¯s sign is called $A$ and Ball¡¯s sign is called $B$). **Ball goes first**.  
After a round of game (a round means that Ball and Alex operates once each in order), if there exists a permutation $p[1..n]$ satisfies that for each $ i \in [1,n]$,$M[i][p[i]]=A$, Alex wins immediately.  
After $\lfloor n^2 /2 \rfloor$ rounds, if Alex hasn¡¯t won, Ball wins instead.  
Notice that whenever anyone tries to mark a marked matrix element(because of forgetting), he will lose the game immediately.  
Sly Ball thinks of a way to interfere Alex. He decides to operate long time after the Alex¡¯s last operation so that Alex may forget about the previous operations.  
Now you get this message and want to know two things for a given $n$: 

* whether Alex has winning strategy if he remembers all the previous operations
* whether Alex has winning strategy if he forgets all the previous operations, and only knows Ball's last operation each time.  

Ball always knows all their previous operations.

## Input Format

Read from the standard input.   
This first line contains a single integer $T$ which means the number of the test cases.   
The following $T$ lines, each line contains one integer $n$ which means the size of the matrix.   

## Output Format

Write to the standard output.  
For each test case, output two lines of `Yes` or `No`.   
The first line means whether Alex can win for sure If he **remembers** the previous operations.  
The second line means whether Alex can win for sure If he **forgets** the previous operations.  


```input1
2
1
2
```

```output1
No
No
No
No
```

```input2
2
1
2
```

```output2
No
No
No
No
```

## Constraints 

For all test cases,  $1\leq n \leq 10^{18}$,$1 \leq T \leq 100$ .

Detailed constraints are as follows (blank grids denote the same constraints as mentioned above):    

|	Subtask	|	Score (percentage)	|	$n$			         	|
|:----------------------:|:----------------:|:------------------------------------:|
|	$1$			|	10		|	$\leq 3$			        |
|	$2$			|	40		|	$\leq 100$			|
|	$3$			|	20		|	$\leq 10^6$			|
|	$4$			|	30		|	$\leq 10^{18}$		|


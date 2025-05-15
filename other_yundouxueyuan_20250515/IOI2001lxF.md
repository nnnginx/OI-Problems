# Description

The Mancala family of games with beads and pits is among the oldest forms of human entertainment. This task introduces a version of the game especially developed for the IOI. The game is played by two players on a round board with seven pits around the edge. In addition, there is a bank for each player.

The game begins by randomly distributing 20 beads into the pits so that each pit contains at least 2 and at most 4 beads. The two players move alternately. To move, the player chooses a non-empty pit and takes all beads out of the pit, and holds them in her hand. As long as there are beads in the player¡¯s hand, she considers the pits in clockwise order, starting one after the emptied one, and performs the following operations:

¡¤ More than one bead in your hand: If the current pit already contains 5 beads, then take one bead out of the current pit and place it into your bank, otherwise place one bead from your hand into the current pit.

¡¤ One bead in your hand: If the current pit contains at least one and at most four beads then move all beads from the pit and the one from your hand into your bank, otherwise (the pit contains 0 or 5 beads) place the bead in your hand into the opponent's bank.

The game is over when after a move all pits are empty and the winner is the player with most beads in her bank.

The starting player always has a winning strategy. You are to write a program, which plays Ioiwari as the starting player and wins. The evaluation opponent plays optimally, that is, once given a chance, it will win and your program will lose.

# Format

## Input and Output

Your program reads input from standard input and writes output to standard output. Your program is player 1, and the opponent is player 2. When your program is started, it must first read a line with 7 integers p ~1~ ,..p ~7~ , the initial number of beads in pits 1,..7, respectively. The pits are labeled with integers from 1 to 7 in clockwise direction on the board. After this, the game starts with empty banks. Your

program should play as follows:

¡¤ If it is your program¡¯s turn to move, then your program should write the label of the pit describing the move to standard output

If it is your program¡¯s opponent¡¯s turn to move, then your program should read the label of the pit defining the move (the pit from which the beads are removed) from standard input.

### **Tools**

You are given a program (ioiwari2 on Linux, ioiwari2.exe on Windows), which plays from one initial game position optimally as Player 2. It will first write to standard output the first line your program is supposed to read, describing the initial values of beads in that game: 4 3 2 4 2 3 2 After this, the program will play the game, trying to read Player 1¡¯s moves from standard input and writing its own moves to standard output. You can run your program and ioiwari2 in separate windows and transfer the conversation manually to both programs. ioiwari2 records the dialogue in the file ioiwari.out.

### **Programming instructions**

In the examples below, you are reading the last integer of the input into variable last and the variable

mymove contains your move.

If you program in C++ and use iostreams, you should use the following implementation for reading standard input and writing to standard output:

cout<<mymove<<endl<<flush; cin>>last;

If you program in C or C++ and use scanf and printf, you should use the following implementation for reading standard input and writing to standard output:

printf("%d\n",mymove); fflush (stdout); scanf ("%d", &last);

If you program in Pascal, you should use the following implementation of reading standard input and writing to standard output:

Writeln(mymove);

Readln(last);

### **Example**

Here is a correct sequence of 6 moves

#### **Pit and bank contents after the operation**

| Operation/Pit label | 1. | 2. | 3. | 4. | 5. | 6. | 7. | Bank1 | Bank2 |
| --------------------- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ------- | ------- |
| Initial situation   | 4  | 3  | 2  | 4  | 2  | 3  | 2  | 0     | 0     |
| Player 1¡¯s move: 2 | 4  | 0  | 3  | 5  | 0  | 3  | 2  | 3     | 0     |
| Player 2¡¯s move: 3 | 4  | 0  | 0  | 4  | 1  | 4  | 0  | 3     | 4     |
| Player 1¡¯s move: 5 | 4  | 0  | 0  | 4  | 0  | 0  | 0  | 8     | 4     |
| Player 2¡¯s move: 4 | 0  | 0  | 0  | 0  | 1  | 1  | 1  | 8     | 9     |
| Player 1¡¯s move: 5 | 0  | 0  | 0  | 0  | 0  | 0  | 1  | 10    | 9     |
| Player 2¡¯s move: 7 | 0  | 0  | 0  | 0  | 0  | 0  | 0  | 11    | 9     |
|  **Scoring**       |    |    |    |    |    |    |    |       |       |

If your program wins a test run, then you get 4 points for that test, a tie in a test gives you 2 points for that test, and otherwise you get 0 points for a test.

### **Solution**

Various parameters (number of the pits, number and distribution of the beads, and especially the game rule) have been tuned to satisfy the following requirements:

¡¤ the game is winnable by the first player

¡¤ not easy to win in most game instances

¡¤ efficient solution possible with reasonable resource limitations (memory and CPU time)

¡¤ draw is possible

¡¤ the number of different game instances is sufficient for testing.

Consider the directed graph whose nodes are the pairs <w, B>, where w is 1 or 2, indicating who is to move next and B is any possible game board (disregarding from the banks). There is an edge from a node <u, A> to a node <v, B> if and only if u + v = 3 and B is obtained from A by a legal move.

Since every move decreases the sum of the beads in the pits, this graph is acyclic.

Let Diff(w, B) be the best score difference for the first player that can be achieved from the game position B, assuming that the second player plays his best. Then

![](file:///C:\Users\ADMINI~1\AppData\Local\Temp\ksohtml6824\wps4.png)0, if B is empty

Diff(w,B)=		Max{Diff(2, Move(B, i)) + D(B, i): for all legal move i}, if w = 1 Min{Diff(1, Move(B, i)) + D(B, i): for all legal move i}, if w = 2,
where Move(B, i) is the board obtained by moving with pit i and D(B, i) is the difference of the number of beads placed in Bank1 and Bank2 when moving with pit i. It is evident, that the first player has winning strategy for a game instance B iff Diff(1, B) > 0.

### **Recursive Algorithm**

The recursive formula for Diff immediately gives a solution to the problem: first player always moves with pit i, which gives the maximum in the formula. It is obvious that this algorithm is not efficient, since it must make a call of Diff before each move. Moreover, the recursive computation recomputes the desired value for a board each time it is accessed.

### **Memoizing algorithm**

We can improve the efficiency of recursive algorithm by storing the values Diff(w, B) once computed. In order to store these values, we assign a unique id number for each possible board. Since during the game, each pit contains at most 5 beads, therefore a board can be uniquely identified by a seven digit base-6 number. The program first computes the optimal value for the sub-problems Diff(w, B) and stores the optimal move in a table. Computation is done by recursion with memoization. During the play, the algorithm looks up for the optimal move in this table.

Space required is 3*MaxN bytes, where MaxN is the largest seven digit base-6 number, which is 279935. We note that the space can be reduced by a factor of 2, if we assign to every board the base-6 number of its rotational equivalent which gives the smallest number.

Time complexity of the algorithm is proportional to the number of edges of the graph (plus initialization of the tables). A rough upper bound is 7*MaxN. In addition to the Memorizing algorithm, we also consider three other attempts to solve the problem. These are required to select the appropriate set of game instances for test.

### **Greedy algorithms**

One can play the game by one step look-ahead greedy strategy. The player always takes those move, which gives the local optimum. Testing of this algorithm shows that for several game instances, the greedy strategy is winning. Making two steps look-ahead gives worth algorithm, it almost always loses the game.

The one step look-ahead greedy algorithm has been implemented in the file owarig1.pas, and two the step look-ahead greedy algorithm in the file owarig2.pas.

### **Random algorithm**

The last attempt is based on randomization, or guessing the right move. Fortunately, the probability of winning a game by doing random choice is very low.

### **Test data**

There are 51 different game instances modulo rotation. The solutions could be tested against all of them, but this is not recommended. The greedy algorithm wins 22 games (if the pit contents in the input are given in the order as listed in the file alldiff.txt) and the number of drawn game is 7. The test cases should be selected according to the intended difficulty level of the task. The test set should contain game instances, that are rotationally equivalent, because of the greedy algorithm might produce different results for them.

Test results for all algorithms are summarized in a table contained in the file alldiff.txt.

Game instances that are recommended for test have been indicated.

### **Time limit**

Time limit should be set to reward time-efficient solutions. This is possible, because the running time of the less efficient solution (recursive algorithm) is larger by an order of magnitude.

### **Library implementations**

The game is implemented in a client server architecture for test runs. The contestant¡¯s program owari and the second player's program player2 executed as separate processes, player2 is the server and owari is the client. The programs communicate using inter-process communication that is implemented by named pipes. This solution is safe and robust.

Only a small library is needed on the client side to implement IPC. Communication is strongly synchronized. Client can only communicate with the server by executing one of the three library operations. The client always sends two integers, the opcode and the operand (possible dummy) and waiting for receiving one integer as a response. The server is listening in a loop for incoming requests, always waiting for two integers (sent by the client), then computes the response and sends it back. The server program starts first and running in background. It is assumed that player2 owned and executed

by a special user which is different from any contestant. It first creates a dummy output file and changes its ownership and permission, so contestant's program can not modify the output file and it will be there even if the client program terminates abnormally. Then opens two pipes, one for input and one for output and listening in a loop for incoming requests on its input pipe.

In case of illegal operand (move) or at the end of the game, the answer sent back makes the client terminate (abnormal or normal, respectively). In case of normal termination, the server closes the pipes and write the output file, after client has been terminated. The client program opens the pipes with appropriate modes at the first call of any of the library operations. If the client initiates its termination or killed because time limit expired, the server terminates due to broken pipe error which is reported on stderr. Therefore, the stderr of both programs should be redirected to files.

Contest-time version is implemented as a single program. The main reason is that IPC is not supported on Windows by gcc/FreePascal. Moreover, it is not important to protect the second player's program (the library) from the contestant program, and the single program version is more convenient for the contestant.

```

```


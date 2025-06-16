## ��Ŀ����
Farmer John and Bessie have devised a new exercise game for the cows.  The cows are running on a circular track of length M (2 <= M <= 1,000,000,000) starting from the same position.  The game proceeds in N (1 <= N <= 14) rounds using a deck of 8N cards each with a number X\_i (0 <= X\_i < M) written on it.

Each round FJ moves the top 8 cards into a separate pile and selects either the top 4 or bottom 4 cards for Bessie to play with.  Bessie then chooses either the top 2 cards or bottom 2 cards of the 4 cards FJ selected.  After this FJ calls out the number on the top card, X\_top, and the cows run a distance of R \* X\_top, where R is the total distance the cows have run so far.  Bessie then calls out the number on the bottom card, X\_bottom, and the cows run a distance of X\_bottom.

FJ is concerned that after the exercise the cows will be too tired to get back to the beginning of the track if they end up too far away.  He believes if the cows end up more than a distance of K (0 <= K <= floor(M/2)) from their starting position they won't be able to get back home.

It is guaranteed that if FJ plays correctly, he will always be able to ensure the cows can come home, irrespective of the moves made by Bessie! For each round, your task is to determine which half of the cards FJ should choose such that no matter what Bessie does from that point on, FJ can always get the cows home.  Bessie will then make the move provided in the input and you can then continue onto the next round.  Note that even though Bessie's moves are provided to you in the input, you are to specify moves for FJ that would have worked no matter what Bessie chooses (so it is effectively as if FJ does not really know what Bessie will do during her moves).


## �����ʽ
\* Line 1: Three space-separated integers N, M, K

\* Line 2: A string N characters.  If the ith character is 'T' it means Bessie will select the top 2 cards in the ith round.  Otherwise the ith character will be 'B' to indicate Bessie will select the bottom 2 cards in the ith round.

\* Lines 3..2+N: Each line contains eight integers representing the 8 cards to be used that round from top to bottom.


## �����ʽ
\* Line 1: A string of N characters where the ith character is 'T' if FJ should choose the top 4 cards or 'B' if FJ should choose the bottom 4 cards in the ith round.  If there are multiple ways to get the cows home, choose the lexicographically first (that is, the string that is alphabetically smallest).


## ��Ŀ����
FJ �ͱ���Ϊ��ţ�������һ���µ��ܲ���Ϸ���ܵ��ǻ��еģ�����Ϊ $(2 \le M \le 1,000,000,000)$ �Ļ��У���ţ������ͬ������λ�á������Ϸһ��Ҫ���� $N\ (1 \le N \le 14)$ �֣�ͨ��һ�� $8N$ �ŵ�ֽ��������ÿһ�ֵ��ܲ����룬ÿ��ֽ�ƶ���һ������ $X_i\ (0 \le X_i<M)$��

ÿһ�֣�FJ ȡ��������� $8$ ��ֽ�ƣ�Ȼ����ȡ���� $8$ �ŵ�������ߵ��µ� $4$ �š����ţ�������� $4$ ������ȡ��������ߵ��µ� $2$ �ţ�����һ�ŵ�����Ϊ $X_{\mathrm{top}}$������һ�ŵ������� $X_{\mathrm{bottom}}$����ţ���� $R\times X_{\mathrm{top}}$ �ľ��루$R$ ��ʾ��ţ���Ѿ��ܹ��ľ��룩������ $X_{\mathrm{bottom}}$ �ľ��롣

FJ ������ţ��̫�۶��ز�����㣬��Ϸ����ʱ������ţ���뿪�����볬�� $K\ (0 \le K \le \lfloor M/2\rfloor)$�������Ǿͻز�������ˡ�

���Ᵽ֤���� FJ ѡ����ȷ��ȡ�Ʋ��ԣ����۱������ȡ�ƣ���ţ�Ƕ��ܹ��ص���㡣����ÿһ�֣���������Ǿ���ȡ�� $4$ ��ֽ�ơ������������У�������ÿ��ѡ������֪�ģ��� FJ ��ÿ��ȡ��ʱ���������ŵ�ѡ��Ӧ�ñ��ٶ�Ϊ��δ֪�ģ������۱�����ôѡ��FJ ��ѡ�����ܱ�֤��ţ���ܹ��ص���㡣

```input1
2 2 0 
TT 
1 0 0 0 0 0 0 1 
0 1 1 1 0 0 1 0 

```

```output1
TB 

```

## ��ʾ
The cows must end up exactly where they started to be able to come home. Note that FJ is not aware of what choices Bessie is going to make beforehand.  If FJ did know, he could have chosen the bottom half each time.



<p>In a n-storey resort a grand party is arranged in the nth floor of the building and two magical elevators A and B are stationed at the ground floor (zero th floor).&nbsp;</p>
<p>There are people waiting in all floors from to 0 to n-1 for attending the party. These two magical elevators are used for getting these people to the party. These elevators can be moved from one floor to any other floor. The time it takes to move any elevator from i th floor to j th floor is abs(j - i) time units.</p>
<p>Also there is a cost associated with moving the elevator from i th floor to j th floor.&nbsp;</p>
<p>If the elevator A moves from floor i to floor j with x people, then cost equals A[i] ^ A[j] ^ x, where '^' is the bitwise XOR operator. Similarly for the elevator B, it is B[i] ^ B[j] ^ x. However, if the lift stops on the k'th floor and 'a' people get on the elevator and 'b' people get off the elevator, to make a new count of 'y' people, then new cost is (A[i] ^ A[k] ^ x) + (A[k] ^ A[j] ^ y). (see notes).</p>

<p>People who are inside the elevator can be made to get down from it at any floor that it stops. It takes zero time for people to get into or out of the elevator.&nbsp;</p>

<p>All persons who are waiting have to be taken to the nth floor. As the party is going to start immediately the resort manager wants everyone to be there in the party in the least time possible. It is your job to control these elevators in such a way that everyone is there in the party in the least time possible and also minimize the cost of controlling these elevators.</p>

<p><strong>Notes:</strong></p>
<p>1. The objective is to get all the people waiting in floors 0, 1....n - 1 to floor n.</p>
<p>2. The elevators can move up or down.</p>
<p>3. It takes zero time for the elevator to stop at any floor and for people to get down or get into the elevator.</p>
<p>4. If Lift A carries 5 persons from 2nd floor to 6th floor, cost = A[2] ^ A[6] ^ 5</p>
<p>5. If 1 more person enters Lift A on the 4th floor, the cost will be (A[2] ^ A[4] ^ 5) + (A[4] ^ A[6] ^ 6)</p>

<h3>Constraints:</h3>
<p>1 &lt;= n &lt;= 30;</p>
<p>The sum of people waiting in all floors won't exceed 1000 and there is atleast one person waiting in every floor from 0 to n-1.</p>
<p>All values of the array A and B are non-negative numbers lesser than or equal to 1000.</p>

<h3>Input</h3>
<p>First Line consists of an integer denoting the number of test cases(atmost 10).</p>
<p>Every test case will be of the following form.</p>
<p>First line contains n the number of floors in the building.</p>
<p>Second line contains n+1 integers: A[0], A[1].....A[n].</p>
<p>Third line contains n+1 integers: B[0], B[1]......B[n].</p>
<p>Fourth line contains n integers: The number of persons waiting in each floor from 0 to n - 1.</p>

<h3>Output</h3>
<p>For every test case output one integer on a new line: the minimum cost for operating the elevators and ensuring that all people reach the n'th floor.</p>

<h3>Example</h3>
<pre><strong>Sample Input:</strong>
2
2
0 1 3
0 1 5
2 1
4
1 3 5 7 9
2 4 6 8 10
1 2 3 4

<strong>Sample Output:</strong>
1
16</pre>

<h3>Explanation</h3>
<p>In the first test case,&nbsp;</p>
<p>1. Lift A carries 1 person from 0th floor to 1st floor. Cost = A[0] ^ A[1] ^ 1 = 0</p>
<p>2. Lift B carries 1 person from 0th floor to 1st floor. Cost = B[0] ^ B[1] ^ 1 = 0</p>
<p>3. The person waiting in 1st floor and person from Lift A both move to Lift B. Lift B carries 3 people from 1st floor to 2nd floor. Cost = B[1] ^ B[2] ^ 3 = 1</p>
<p>4. All persons have reached the party in 2 time units and incurring a cost of 1.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
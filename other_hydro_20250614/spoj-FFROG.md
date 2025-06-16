<p>WiseFrog, The King of FrogLand is on his Deathbed. He has 2 Sons, SensibleFrog and SmartFrog. Both of them are "Infinitely Intelligent". To decide who will succeed him as King, he devises a Strategy Game for the two Sons-<br><br>

An Arena is constructed, in the form of a Rectangle, having m X n Square Areas. They are labelled as (i,j), starting from the Upper Left extremity of the Arena [i=0,1,2...n-1; j=0,1,2...m-1]. The Squares in the Arena are filled with Flying Frogs, in a Random Manner, such that there can be any number of Frogs in each square.<br><br>

Once the Arena is ready, the 2 Frog Princes begin to play the Game, which is played in the following manner: SensibleFrog, being the King's favourite, starts the Game.<br><br>

Each Prince takes his turn alternately. In his turn, he is permitted a maximum of K moves, and a minumum of 1 move. A "Move" is defined as the Issuing of an Order to any Frog of his choice. The "order" consists of the Direction to jump in, and the Number of Squares to Cover ( which should be positive ), the directions of movement permitted being Up and Left Only. However, the Order must not be such that it causes the Frog to land outside the Arena. Being Flying Frogs, the frogs in the Arena can jump any distance without trouble.<br><br>

If there arrives a situation where the Prince having his turn does not have ANY move Possible ( that is, ALL the Flying Frogs are already at the top-left most square of the arena ), the other Prince is declared the Winner. Given all the Starting Conditions, your task is to find out who becomes the King of FrogLand.<br>

</p><h3>Input</h3>
<p>First line of input contains an integer T, equal to the number of test cases. Followed is the description of each of the T test cases and you are required to process all test cases. First line of each test case contains three integers m,n,k ( in this order ). Each of the next m lines contain n integers separated by spaces. Jth integer in ith line corresponds to the number of Flying Frogs in Square (i,j) in the arena.

</p><h3>Output</h3>
<p>Output contains one line for each test case. You have to output "SensibleFrog Wins!." if SensibleFrog wins and "SmartFrog Wins!." otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
1 1 1
837465
2 2 1
0 0
0 1
2 2 2
0 0
0 2


<b>Output:</b>
SmartFrog Wins!.
SmartFrog Wins!.
SensibleFrog Wins!.

</pre>

<h3>Constraints and Limits</h3>
<p>T �� 20, 1 �� m,n �� 1000, m*n �� 10^5, 1 �� k �� 10^9 , 0 �� Number of Frogs in a square �� 10^100.<br>
The total input data in each of the input file doesn't exceed 5 MB.
</p>
<p>Heroes... ugh...<br><br>My plan to destroy the world was almost finished, but now heroes have gathered in their last attempt to save the earth (which, as everybody knows, is pretty flat). Heroes formed a defensive <strong>N</strong> * <strong>M</strong> grid, each of the N * M heroes stands in one position of the grid. Also, the hero in position <strong>i,j</strong> has h<sub>ij</sub> life points.<br><br>Of course, they stand no chace against my wrath. I'll attack them with <strong>Q</strong> spells, the i-th spell will have power p<sub>i</sub> and will attack the submatrix with corners (r1<sub>i</sub>, c1<sub>i</sub>) and (r2<sub>i</sub>, c2<sub>i</sub>). Heroes can decide how to distribute the power of the spell over the heroes in the attacked submatrix, so, for each spell, each hero of the submatrix will decrease his life points by a number of integer points (possibly zero), such that between all the heroes of the submatrix take all the p<sub>i</sub> points of damage. Of course, a hero can only take more damage if his life is greater than zero. Note that the damage they receive will accumulate over all the Q spells.<br><br>If heroes cannot receive the damage points of a spell, my spell will reach the (flat) earth and immediately destroy it.<br><br>Assuming heroes know the sequence of spells I'll use, can they save the earth if they work optimally?</p>
<h3>Input</h3>
<p>In the first line, two integers, N and M , the number of rows and columns in the grid.</p>
<p><br>Next N lines, each one contains M integers h<sub>ij</sub> , the initial life points of each hero.</p>
<p><br>Then a line with integer Q, the number of spells.</p>
<p><br>Then follow Q lines, each with 5 integers: r1<sub>i</sub> , c1<sub>i</sub> , r2<sub>i</sub> , c2<sub>i</sub> , p<sub>i</sub> .</p>
<h3>Output</h3>
<p>Print ”BOOM!” (without quotes) if the earth is destroyed, print ”ugh” (without quotes) otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 3<br>2 1 3<br>2 4 4<br>2<br>1 1 2 2 7<br>1 2 2 3 9

<strong>Output:</strong>
ugh<br><br><strong>Input:<br></strong>2 3<br>2 1 3<br>2 4 4<br>2<br>1 1 2 2 7<br>1 2 2 3 10<br><br><strong>Output:<br></strong>BOOM!<br></pre>
<h3>Constraints<br><br></h3>
<p>• 1 ≤ N ≤ 10</p>
<p>• 1 ≤ M ≤ 10000</p>
<p>• 1 ≤ Q ≤ 500</p>
<p>• 1 ≤ r1<sub>i</sub> ≤ r2<sub>i</sub> ≤ N</p>
<p>• 1 ≤ c1<sub>i</sub> ≤ c2<sub>i</sub> ≤ M</p>
<p>• 1 ≤ p<sub>i</sub> , h<sub>ij</sub> ≤ 10<sup>4</sup></p>
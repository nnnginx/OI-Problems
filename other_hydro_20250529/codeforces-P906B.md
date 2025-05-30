## Description

<div><p>Students went into a class to write a test and sat in some way. The teacher thought: "Probably they sat in this order to copy works of each other. I need to rearrange them in such a way that students that were neighbors are not neighbors in a new seating."</p><p>The class can be represented as a matrix with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns with a student in each cell. Two students are neighbors if cells in which they sit have a common side.</p><p>Let's enumerate students from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i>·<i>m</i></span> in order of rows. So a student who initially sits in the cell in row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span> has a number <span class="tex-span">(<i>i</i> - 1)·<i>m</i> + <i>j</i></span>. You have to find a matrix with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns in which all numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i>·<i>m</i></span> appear exactly once and adjacent numbers in the original matrix are not adjacent in it, or determine that there is no such matrix.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span"><i>n</i>·<i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rows and the number of columns in the required matrix.</p></div><div class="output-specification"><p>If there is no such matrix, output "<span class="tex-font-style-tt">NO</span>" (without quotes). </p><p>Otherwise in the first line output "<span class="tex-font-style-tt">YES</span>" (without quotes), and in the next <span class="tex-span"><i>n</i></span> lines output <span class="tex-span"><i>m</i></span> integers which form the required matrix.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span"><i>n</i>·<i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rows and the number of columns in the required matrix.</p>

## Output

<p>If there is no such matrix, output "<span class="tex-font-style-tt">NO</span>" (without quotes). </p><p>Otherwise in the first line output "<span class="tex-font-style-tt">YES</span>" (without quotes), and in the next <span class="tex-span"><i>n</i></span> lines output <span class="tex-span"><i>m</i></span> integers which form the required matrix.</p>

## Samples

```input1
2 4

```

```output1
YES
5 4 7 2 
3 6 1 8 

```






```input2
2 1

```

```output2
NO

```




## Note

<p>In the first test case the matrix initially looks like this:</p><pre class="verbatim"><br>1 2 3 4<br>5 6 7 8<br></pre><p>It's easy to see that there are no two students that are adjacent in both matrices.</p><p>In the second test case there are only two possible seatings and in both of them students with numbers 1 and 2 are neighbors.</p>

<p></p><p align="justify">
Word puzzles are usually simple and very entertaining for all ages.
They are so entertaining that Pizza-Hut company started using table
covers with word puzzles printed on them, possibly with the intent to
minimise their client's perception of any possible delay in bringing
them their order.

</p><p align="justify">
Even though word puzzles may be entertaining to solve by hand, they
may become boring when they get very large. Computers do not yet get
bored in solving tasks, therefore we thought you could devise a
program to speedup (hopefully!) solution finding in such puzzles.

</p><p align="justify">
The following figure illustrates the PizzaHut puzzle. The names of the
pizzas to be found in the puzzle are: <font size="-1">MARGARITA, ALEMA,
  BARBECUE, TROPICAL, SUPREMA, LOUISIANA, CHEESEHAM, EUROPA, HAVAIANA,
  CAMPONESA</font>.  

</p><p>

</p><div align="CENTER"><table cellpadding="3" border="1">
<tbody><tr><td align="LEFT" valign="TOP" width="6"><font size="-1">
 </font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">0</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">1</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">2</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">3</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">4</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">5</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">6</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">7</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">8</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">9</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">10</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">11</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">12</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">13</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">14</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">15</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">16</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">17</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">18</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">19</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 

0</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Y</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
1</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">X</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">F</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">V</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>

</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
2</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Z</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">X</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">V</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
3</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Z</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">X</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Z</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
4</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">F</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
5</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
6</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
7</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">V</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Z</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
8</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">F</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
9</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Y</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">F</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">X</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
10</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">Y</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">V</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
11</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
12</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">D</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">V</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Z</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
13</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
14</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">F</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">X</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
15</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">D</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Y</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Y</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">X</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
16</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">K</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
17</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Y</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">J</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Q</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">W</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">D</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">G</font></td>
</tr>

<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
18</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">U</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">Y</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">R</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">E</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">T</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">M</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
</tr>
<tr><td align="LEFT" valign="TOP" width="6"><font size="-1"> 
19</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">F</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">C</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">O</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">H</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">V</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">I</font></td>

<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">N</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">A</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">L</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">B</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">P</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">F</font></td>
<td align="LEFT" valign="TOP" width="3"><font size="-1">S</font></td>
</tr>

</tbody></table></div>

<h3>Problem</h3>

<p align="justify">
Your task is to produce a program that given the word puzzle and words
to be found in the puzzle, determines, for each word, the position of
the first letter and its orientation in the puzzle.

</p><p align="justify">
You can assume that the left upper corner of the puzzle is the origin,
<it>(0,0)</it>. Furthemore, the orientation of the word is marked clockwise
starting with letter <tt>A</tt> for north (note: there are 8 possible
directions in total).
</p><h3>Input</h3>
<p></p><p>
The first line of the input contains a number <it>T ¡Ü 10 which indicates the number of test cases to follow.
Each test case starts with a line consisting of three positive numbers: The
number of lines of the word puzzle, <it>0 &lt; L ¡Ü 1000</it>, the number of columns,
<it>0 &lt; C ¡Ü 1000</it>, and the number of words to be found, 
<it>0 &lt; W ¡Ü 1000</it>. The following <it>L</it> input lines, each
 consisting of <it>C</it> uppercase letters, contain
the word puzzle. Then at last the <it>W</it> words are input one per line. You can assume that each word can be found exactly once in the word puzzle.

</it></p><h3>Output</h3>
<p align="justify">
For each test case your program should output <it>W</it> lines: For each word (using the same order as the
words were input) print a triplet defining the coordinates, line and column,
where the first letter of the word appears, followed by a letter
indicating the orientation of the word according to the rules defined
above. Each value in the triplet must be separated by one space only.<br>
<b>Print one blank line between test cases.</b>

</p><h3>Example</h3>

<pre><b>Input:</b>

1
20 20 10
QWSPILAATIRAGRAMYKEI
AGTRCLQAXLPOIJLFVBUQ
TQTKAZXVMRWALEMAPKCW
LIEACNKAZXKPOTPIZCEO
FGKLSTCBTROPICALBLBC
JEWHJEEWSMLPOEKORORA
LUPQWRNJOAAGJKMUSJAE
KRQEIOLOAOQPRTVILCBZ
QOPUCAJSPPOUTMTSLPSF
LPOUYTRFGMMLKIUISXSW
WAHCPOIYTGAKLMNAHBVA
EIAKHPLBGSMCLOGNGJML
LDTIKENVCSWQAZUAOEAL
HOPLPGEJKMNUTIIORMNC
LOIUFTGSQACAXMOPBEIO
QOASDHOPEPNBUYUYOBXB
IONIAELOJHSWASMOUTRK
HPOIYTJPLNAQWDRIBITG
LPOINUYMRTEMPTMLMNBO
PAFCOPLHAVAIANALBPFS
MARGARITA
ALEMA
BARBECUE
TROPICAL
SUPREMA
LOUISIANA
CHEESEHAM
EUROPA
HAVAIANA
CAMPONESA

<b>Output:</b>

0 15 G
2 11 C
7 18 A
4 8 C
16 13 B
4 15 E
10 3 D
5 1 E
19 7 C
11 11 H
</pre>
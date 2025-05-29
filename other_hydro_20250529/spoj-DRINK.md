<p>

A good drink is always served on ice.
That said, the amount of ice is what makes the difference.
If it is too much, the drink will be well cooled, however, this is a bit of fraud as there could be less ice (and more Vodka for example).
On the other hand, if there is too little ice the drink is warm which is unacceptable.
You are to help the bartender, of course neither with mixing nor drinking, but with calculating the expected outcome of such mixtures.

</p><p>

To make things easier, we assume that pure water is mixed with ice in a closed system, i.e., there is no problem with the outside temperature or the warming of the bottle, etc.
Therefore, after a some time has passed, the system may be regarded as balanced (there is no further change in temperature and no more melting or freezing).
Your job is to calculate the final temperature of this balanced system and the amount of ice and water in this equilibrium state.

</p><p>

As you know from physics, it takes 4.19 Joule to heat one gram of water one Kelvin, whereas it takes 2.09 Joule if it is ice.
We define the capacities <code>c<sub>w</sub> = 4.19 J/(g*K)</code> and <code>c<sub>i</sub> = 2.09 J/(g*K)</code>.
Melting one gram of ice takes 335 Joule, where the temperature remains constant at zero.
We define the constant <code>e<sub>m</sub> = 335 J/g</code>.
The total thermal energy of the ice and the water before the experiment is equal to the thermal energy of the final mixture.


</p><p>

The figure below shows the energy of one gram of ice, ice-water-mixture, or water, where the temperature is measured relative to -30 degrees Celsius.
The jump at 0 degrees represents the melting of ice to water.
The amount of energy gained is proportional to the amount of ice already melted.

</p><h3>Input Specification</h3><p>

The input contains several test cases.
Each test case consists of four real numbers <code>m<sub>w</sub>, m<sub>i</sub>, t<sub>w</sub>, t<sub>i</sub></code>.
The mass of water <code>m<sub>w</sub></code> and the mass of ice <code>m<sub>i</sub></code> are both non-negative, given in grams, and <code>m<sub>w</sub> + m<sub>i</sub> &gt; 0</code>.
The water temperature <code>t<sub>w</sub></code> and the ice temperature <code>t<sub>i</sub></code> follow, both given in degrees Celsius, and you may assume that <code>-30 &lt; t<sub>i</sub> &lt;= 0 &lt;= t<sub>w</sub> &lt; 100</code>.
The last test case is followed by four zeroes.


</p><h3>Output Specification</h3><p>

For each test case output the amount of ice and water in grams and the final temperature of the mixture in degrees Celsius.
All numbers must be rounded to one digit.
Adhere to the sample output for the exact format to use.

</p><p>

</p><table cellpadding="0" cellspacing="0" width="100%"><tbody><tr>

<td valign="top">
<h3>Sample Input</h3><p>

</p><pre>100 20 50 -10
100 22 0  0
100 35 25 -10.5
10  90 25 -28
0 0 0 0
</pre>

<h3>Sample Output</h3><p>

</p><pre>0.0 g of ice and 120.0 g of water at 27.5 C
22.0 g of ice and 100.0 g of water at 0.0 C
6.0 g of ice and 129.0 g of water at 0.0 C
100.0 g of ice and 0.0 g of water at -4.2 C
</pre>
</td>

<td align="right" valign="top">
<img src="./22233/file/jrlZymQP.png">
</td>

</tr></tbody></table>
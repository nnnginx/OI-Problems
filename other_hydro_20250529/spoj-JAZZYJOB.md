<p>With the magnification of the Energy Crisis, Chemists have decided to re-examine the existing procedures of preparation of various Chemical Substances.<br><br>

As part of this Project, they list all the elements that they commonly find as raw material (Initial Reactants), and the ones that they intend to produce (Final Products). They also prepare an extensive list of the various known reactions/processes that are used to convert one substance to another.<br><br>

One major issue that they find is that the Initiation of many reactions needs absurdly large amounts of energy. They wish to keep low the activation energies used in the new procedures.<br><br>

Knowing all this, they now attempt to find out such methods of preparing the target substances :<br>

(1) in which the highest value of activation energy needed by any of the reactions that make up the path, in any of the methods, does not exceed a given upper value,<br>
(2) which minimizes the Total reactions/procedures performed in All the (Initial Reactant) --&gt; (Final Product) conversions.<br><br>

Each substance, on being given a specific amount of energy, converts into some other substance. The formed substance is unique for a particular value of Energy. The process of creating each successive Target Substance (Final Product) starts from one of the Source Substances Only, and leaves no by-products.<br><br>

Your task is to find the minimum value of upper bound such that all final products are obtainable with that upper bound and for this minimum value, find out the minimum
number of conversions to get all the final products. <br><br>

<b>Note:</b> None of the procedures are Reversible, unless explicity stated. Also, if a procedure Is reversible, the Energy requirement may or may not be same. You may assume that there is a limitless supply of the Initial Reactants.<br>


</p><h3>Input</h3>
<p>The first line contains an integer t which is the number of test cases. Each test case begins with a line containing three integers : number of Initial eactants(S), Final Products(D) and the total number of elements (N). Then S+D lines follow, first S lines contain IDs of Initial reactant ( 0 based ) and next D lines contain ID's of Final products ( 0 based). Then follows a line containing an integer R which is number of reactions possible. Then follow R lines, each containing three integers, the Substance(S), the converted substance(C) and the activation energy(A) units required for the reaction. 0 ¡Ü S,C  &lt; n.

</p><h3>Output</h3>
<p>For each test case , output in a different line ,2 integers (a,b) separated by spaces where a is the minimum upper value and b is the minimum number of conversions required for corresponding a. In case that all final products are not obtainable for any value of upper bound, Print a single line with message "Excessive Energy.".

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2 2 6
1
3
0
3
6
1 2 2
2 4 3
4 5 1
4 2 2
3 0 4
5 0 1


<b>Output:</b>
3 4
</pre>

<h3>Constraints and Limits</h3>
<p>N ¡Ü 10000, S ¡Ü N,D ¡Ü N,R &lt; 100000 0 &lt; A &lt; 1000000000
</p>
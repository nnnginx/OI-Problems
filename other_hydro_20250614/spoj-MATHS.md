<p>One could define mathematics as the study of quantity, structure, space and change and as the science of infinity. Sometimes very abstract, mathematics finds nevertheless applications in many engineering domains. The figure below shows so-called Ford circles. These circles are disjoint or tangent and fill the space in a very compact way! Starting with large circles, the space between these circles can be filled with circles of smaller diameter, and so on and so forth.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/imuteb:mathematics" alt="" width="500" height="375"></p>
<p>&nbsp;</p>
<p>Mathematicians observed that the diameters and positions of the centers of these circles follow a given scheme, which can be described with the help of Farey sequences. The Farey sequence of order<em> N</em> is the sequence of completely reduced fractions between 0 and 1, which have denominators less than or equal to <em>N</em>, arranged in increasing size. Thus each Farey sequence starts with the value 0, denoted by the fraction <sup>0</sup>⁄<sub>1</sub>, and ends with the value 1, denoted by the fraction <sup>1</sup>⁄<sub>1</sub>.</p>
<p>The Amazing Circle Mathematicians (ACM) are interested in the number of terms contained in such a Farey sequence as well as in certain precise terms, which they name Interesting and Curious Position In Circle (ICPC). Your job is to provide the ACMs with this abstract information, which helps them to better understand the Ford circles.</p>
<p>&nbsp;</p>
<p><strong>INPUT</strong></p>
<p>The input consists of several test-cases, one per line. Each test-case consists of two numbers, the first is the order <em>N</em> (2&lt;=<em>N</em>&lt;=10<sup>6</sup>) of the Farey sequence the ACM is interested in and the second is the ICPC <em>P</em> (1&lt;=<em>P</em>&lt;=10<sup>4</sup>) . Input terminates on a line containing 0 0 which must not be processed.</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>For each test-case, output first the ICPC, then the total number of terms in the given Farey sequence.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p>2 2</p>
<p>6 12</p>
<p>14 35</p>
<p>0 0</p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p>1/2 3</p>
<p>5/6 13</p>
<p>6/11 65</p>
<p>&nbsp;</p>
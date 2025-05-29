<p align="justify">You must be familiar with the use of numeric k<!-- -->ey<!-- -->s to enter alp<!-- -->habets in mobile phones. A single numeric key when pressed gives a character. W<!-- -->hen pressed again, it changes to another and so on. Once the set of characters mapped to the key is exhausted, the key wraps around to the original<!-- --> characte<!-- -->r<!-- -->.</p>
<p align="justify">The key mapping in this problem is the T9 mapping, restricted to lowercase english characters. The characters corresponding to the individual keys are:</p>
<ul>
<li> 2: a,b,c </li>
<li> 3: d,e,f </li>
<li> 4: g,h,i </li>
<li> 5: j,k,l </li>
<li> 6: m,n,o </li>
<li> 7: p,q,r,s </li>
<li> 8: t,u,v </li>
<li> 9: w,x,y,z </li>
</ul>
<p align="justify">For example, if you press the key 2 once, it prints the character 'a'. On pressing it again, it becomes 'b', then 'c', then back to 'a' and so on.</p>
<p align="justify">Consider a string made of lowercase letters only. To enter this string into a mobile phone, a certain key sequence has to be entered with sufficient gaps in between. Suppose that the key sequence entered is correct but the gaps between keypresses are made arbitrarily. This can result in very different strings being printed.</p>
<p align="justify">For example, let the string to be input be "mod". The key sequence corresponding to this is 6_6663 where '_' denotes a gap between the keypresses. Suppose the keys are pressed in the same order, but with gaps between keypresses arbitrary. This can result in 8 different strings: "mod", "nnd", "omd", "mmmmd", "mnmd", "mmnd", "nmmd" and "md".</p>
<p align="justify">Given an input string, Find the number of possible strings printed by the key sequence corresponding to it.</p>
<h3>Input</h3>
<p align="justify">The first line of the input consists of T, the number of testcases (1��T��10). Following this are T lines, each containing a string. The string will consist only of lowercase letters and will have a maximum length of 100000</p>
<h3>Output</h3>
<p align="justify">For each string, output the number of strings corresponding to its key sequence. Since the answer can be very big, output it modulo 100000007</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
mod
iopc

<strong>Output:</strong>
8
64
</pre>
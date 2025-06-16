<p><span style="font-style: italic;">[The original version of this problem (in Spanish) can be found at&nbsp;</span><a style="font-style: italic;" href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a><span style="font-style: italic;">]</span></p>
<p>GigaFarma is one of the largest pharmaceutical companies in the&nbsp;world, and it is currently conducting experiments using alien&nbsp;DNA. Its goal is to produce a chain of alien DNA that will&nbsp;report the maximum possible benefit when commercialized.</p>
<p>A chain of <em>alien</em> DNA can be understood as a non-empty sequence&nbsp;of genes connected by links, and in turn each <em>gene</em> is a&nbsp;non-empty sequence of bases. Because not every possible&nbsp;sequence of bases corresponds to a valid gene, GigaFarma has&nbsp;created a catalogue of genes that appear in alien DNA, which&nbsp;are the only ones considered valid sequences of bases. Each of&nbsp;these genes has a <em>value</em> according to its functionality, and a&nbsp;given chain of alien DNA has a <em>market value</em> that is the sum of&nbsp;the values of the genes that compose it.</p>
<p>We will represent the different <em>bases</em> with lowercase letters,&nbsp;<span style="font-family: 'courier new', courier;"><strong>'a'</strong></span>-<span style="font-family: 'courier new', courier;"><strong>'z'</strong></span>, and <em>links</em> using a hyphen <span style="font-family: 'courier new', courier;"><strong>'-'</strong></span>. In the following example&nbsp;we can see on the left a possible list of genes and their&nbsp;corresponding values; on the right there are some chains of&nbsp;alien DNA that can be formed with these genes, along with their&nbsp;corresponding market values.</p>
<p style="text-align: center;"><img title="TAP2012G1" src="../../content/fidels:TAP2012G1" alt="TAP2012G1"></p>
<p>GigaFarma can only produce very specific DNA chains, which we&nbsp;call <em>producible</em>. These chains are a non-empty sequence of DNA&nbsp;portions that the company can synthesize, joined without any&nbsp;additional links between them. Each <em>portion </em>is a sequence of&nbsp;bases and links containing at least one link, but without any&nbsp;consecutive, initial or final links. Each portion has a given&nbsp;<em>cost</em>, determined by the difficulty associated to its&nbsp;production, so each producible chain of DNA has a <em>production&nbsp;cost</em> that is the sum of the costs of each of the portions that&nbsp;form it. In the following example, we can see on the left a&nbsp;list of DNA portions and their costs; on the right we have some&nbsp;producible chains of DNA that can be formed with these&nbsp;portions, along with their associated production cost.</p>
<p style="text-align: center;"><img title="TAP2012G2" src="../../content/fidels:TAP2012G2" alt="TAP2012G2"></p>
<p>Note that there might be multiple ways of forming the same&nbsp;producible chain using different portions. This is the case of&nbsp;<span style="font-family: 'courier new', courier;"><strong>"como-como-les"</strong></span> in the example, which can be obtained using&nbsp;portions <span style="font-family: 'courier new', courier;"><strong>"como-co"</strong></span> and <span style="font-family: 'courier new', courier;"><strong>"mo-les"</strong></span> with a production cost of <strong>7</strong>, or&nbsp;just using <span style="font-family: 'courier new', courier;"><strong>"como-como-les"</strong></span> with a production cost of <strong>12</strong>. Of&nbsp;course, when there is more than one way to synthesize a given&nbsp;producible chain of DNA, GigaFarma will always do so using the&nbsp;cheapest possible process.</p>
<p>&nbsp;</p>
<p>Clearly, the set of alien DNA chains is infinite, just like the&nbsp;set of producible DNA chains. However, GigaFarma is not&nbsp;directly interested in any of these sets, but in their&nbsp;intersection. If we check the previous examples, we can see&nbsp;that <span style="font-family: 'courier new', courier;"><strong>"como-les"</strong></span> is a valid alien DNA chain, but is not&nbsp;producible; <span style="font-family: 'courier new', courier;"><strong>"mo-les"</strong></span> is producible, but is not an alien DNA&nbsp;chain; and <span style="font-family: 'courier new', courier;"><strong>"como-como-les"</strong></span> is both. For each alien and&nbsp;producible DNA chain, the company can commercialize this chain&nbsp;to get a <em>net benefit</em> that equals the market value of this chain&nbsp;minus its production cost. Of course, if this net benefit is&nbsp;not positive, the corresponding chain will never be produced.</p>
<p>Because there is so much genetic material all over the place,&nbsp;GigaFarma would pay anything in order to know what is the&nbsp;maximum net benefit it can obtain for some producible and alien&nbsp;DNA chain.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">Each test case is described using several lines. The first line</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">contains two integer numbers G and P, representing the number</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">of genes in the catalogue and the number of portions GigaFarma</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">can produce (1 &lt;= G, P &lt;= 100).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">Each of the following G lines describes a different gene using</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">a string S and an integer V. The string S has between 1 and 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">characters, and is formed solely by lowercase letters</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">representing the bases that form this gene; the integer V</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">represents the value of this gene (1 &lt;= V &lt;= 1000).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">Each of the following P lines describe a different DNA portion,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">using a string T and an integer C. The string T has between 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">and 30 characters, and is composed of lowercase letters and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">hyphens only, respectively representing the bases and links in</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">this portion. T contains at least one link, but will never have</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">initial, final or consecutive links. The integer C represents</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">the production cost for the corresponding portion (1 &lt;= C &lt;=</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">1000).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">Note that in every test case, all the genes are different from</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">one another, and all the portions are different from one</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">another. The end of the input is signalled by a line containing</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 182px; width: 1px; height: 1px; overflow: hidden;">two times the number -1</div>
<p>Each test case is described using several lines. The first line&nbsp;contains two integer numbers <strong>G</strong> and <strong>P</strong>, representing the number&nbsp;of genes in the catalogue and the number of portions GigaFarma&nbsp;can produce (<strong>1 ��&nbsp;G, P&nbsp;</strong><strong>��</strong><strong>&nbsp;100</strong>).</p>
<p>Each of the following <strong>G</strong> lines describes a different gene using&nbsp;a string <strong>S</strong> and an integer <strong>V</strong>. The string <strong>S</strong> has between <strong>1</strong> and <strong>10</strong>&nbsp;characters, and is formed solely by lowercase letters&nbsp;representing the bases that form this gene; the integer <strong>V</strong>&nbsp;represents the value of this gene (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;V&nbsp;</strong><strong>��</strong><strong>&nbsp;1000</strong>).</p>
<p>Each of the following <strong>P</strong> lines describe a different DNA portion,&nbsp;using a string <strong>T</strong> and an integer <strong>C</strong>. The string <strong>T</strong> has between <strong>1</strong>&nbsp;and <strong>30</strong> characters, and is composed of lowercase letters and&nbsp;hyphens only, respectively representing the bases and links in&nbsp;this portion. <strong>T</strong> contains at least one link, but will never have&nbsp;initial, final or consecutive links. The integer <strong>C</strong> represents&nbsp;the production cost for the corresponding portion (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;C&nbsp;</strong><strong>��</strong><strong>&nbsp;1000</strong>).</p>
<p>Note that in every test case, all of the genes are different from&nbsp;one another, and all of the portions are also different from one&nbsp;another. The end of the input is signalled by a line containing&nbsp;two times the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you should print a single line containing&nbsp;an integer number, representing the maximum net benefit that&nbsp;GigaFarma can obtain from a producible and alien DNA chain. If&nbsp;no net benefit is positive, you should print the value 0. If&nbsp;the net benefit can be arbitrarily large, you should print an&nbsp;asteris <strong><span style="font-family: 'courier new', courier;">'*'</span></strong>.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4 6
hola 5
como 5
les 3
va 2
como-co 3
mo-co 8
mo-les 4
como-como-les 12
ta-no-sirven 100
hasta-es 200
2 3
xyz 1000
zyxxyz 1000
xyz-zyx 1
zyx-xyz 1
xyz-xyz-zyx-xyz 1
2 1
abc 1
abcabc 1000
abc-abc 999
1 1
ser 10
no-ser 5
-1 -1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">6
0
*
0</span><span style="white-space: normal;">
</span></pre>
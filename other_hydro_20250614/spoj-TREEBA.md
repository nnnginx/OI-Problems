<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Hakeri prisluškuju komunikaciju Mirka i Slavka te pokušavaju razumjeti presretnute poruke. Rječnik Mirka i Slavka sadrži M riječi te se svaka poruka koju jedan od njih pošalje drugome sastoji od niza riječi iz rječnika odvojenih razmacima. Međutim, poruke koje hakeri presreću su zbog slabe kvalitete njihove opreme izmjenjene na sljedeći način:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1. U poruku je umetnuto najviše K šumova – proizvoljnih nizova slova. Svaki šum je uvijek umetnut između dvije riječi ili prije prve ili nakon zadnje riječi, dakle nikad unutar neke riječi.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2. Svi razmaci između riječi u poruci su izbrisani.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Na primjer ako Mirko pošalje poruku 'mirko slavko', kada je hakeri presretnu ona može biti 'mirkoxyzslavko', gdje je niz 'xyz' šum, a riječi 'mirko' i 'slavko' se nalaze u rječniku. Hakerima je poznat njihov rječnik te su upravo zaprimili novu izmjenjenu poruku koju žele rastaviti na riječi iz riječnika i šumove. Od svih mogućih načina na koji se to može napraviti zanima ih onaj gdje ima najviše moguće riječi iz rječnika. Napišite program koji za zadani rječnik, zadani broj K, te zaprimljenu izmjenjenu poruku dobivenu na opisani način, određuje koliko najviše može biti riječi iz rječnika u rastavu, te određuje jedan (bilo koji) rastav u kojem je najviše moguće riječi iz rječnika.</div>
<p>Hackers are eavesdropping communication beetwen Mirko and Slavko and trying to understand the intercepted messages.</p>
<p>Dictionary from Mirko and Slavko contains M words and every message which one of them send to another consists of a series of words from dictionary separated by spaces.</p>
<p>However, the messages which hackers are intercepting due to poor quality of their equipment are changed as follows:</p>
<ol>
<li>In the message are inserted at most K noises - arbitrary strings of letters. Every noise is always inserted between two words or before the first or after the last word and never within a word.&nbsp;</li>
<li>All spaces between the words in the message are deleted.&nbsp;</li>
</ol>
<p>For example, if Mirko sends a message 'mirko slavko', when hackers intercept it, it can be 'mirkoxyzslavko', where 'xyz' is a noise, and the words 'mirko' and 'slavko' are found in the dictionary.</p>
<p>Hackers know their dictionary and have just received a new altered message which they want to disassemble to the dictionary words and sounds. Of all possible ways in which they can do that, they are interested in the one which has the most words from the dictionary.</p>
<p>Write a program that, given the dictionary, the number K, and received a modified message obtained as described above, determines a way in which the most words from dictionary are used.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains number T ( 1&nbsp;≤&nbsp;T ≤&nbsp;12 ) - the number of test cases.</p>
<p>The second line contains two integers M (1 ≤ M ≤ 1000) and K (0 ≤ K ≤ 10) - the number of words in the dictionary and the maximum amount of noise in each received message.&nbsp;</p>
<p>The third line is the text messages received - a series of lowercase letters of length N (1 ≤ N ≤ 10 000). Each of the following M lines contains a word in the dictionary - a series of at least one and a maximum of 20 lowercase letters.</p>
<h3>Output</h3>
<p>In the first line of output write maximum number of words from the dictionary in disassembled message.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>1</pre>
<pre>5 3 
prisluskujuabcdnassumhakeri 
mirko 
nas 
slavko 
hakeri 
prisluskuju</pre>
<pre><strong>Output:</strong>
3</pre>
<p><strong>Explanation: One of the m</strong><strong>essages is 'prisluskuju #### nas ### hakeri' which has two noises, and maximum of three words.</strong></p>
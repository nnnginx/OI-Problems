<p>Heta is a conventional name for the historical Greek alphabet letter Eta (¦§) and several of its variants, when used in their original function of denoting the consonant /h/ (Wikipedia). Because of whispers of N'Zoth the corruptor, Heta now wants to destroy all existing alphabets (fiction).</p>
<p>Heta has a spell book containing spells to delete a string. There are several spells in that book. Armed with the spellbook, Heta starts his journey to complete his mission.  On his way, Heta found a very long string. To delete that string, Heta reads that string letter by letter from the first letter. If at any point he found a substring that's present in his spellbook, that spell will be cast and that substring will be destroyed. Then he continues until he reach the end of that string and no more spell can be used. If there are multiple spells that can be used in one time, the spell that appears first in the book is used. Determine what's left of the very long string after Heta is done!</p>
<h3>Input</h3>
<p>First line is a string containing A-Z. String can contain from 1 to 100000 characters. Next line of input is N, the number of spells in the spellbook (1 <span style="text-decoration: underline;">&lt;</span><span style="text-decoration: underline;">&nbsp;</span>N <span style="text-decoration: underline;">&lt;</span>&nbsp;100). Next N lines contain spells sorted by appearance in the spellbook. Each spell is a string containing A-Z with a length from 1 to 100.</p>
<h3>Output</h3>
<p>One line containing the string after Heta is done doing his magic.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
KUKUKAKIKUKAKEKKUKAKAKKUKAKUKAKU
2
KEK
UK

<strong>Output:</strong>
KAKIKAKAKAKKAKAKU

<strong>Input:</strong>
HEATHLEDGER
2
HEATH
LEDGER

<strong>Output:</strong>


<strong>Input:</strong>
KAPKAPPAPAK
1
KAPPA

<strong>Output:</strong>
K

<strong>Input:</strong>
CABAI
3
ABA
AB
B

<strong>Output:</strong>
CAI
</pre>
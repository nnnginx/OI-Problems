<p>Nowadays, people who want to communicate in a secure way use asymmetric encryption algorithms such as RSA. However, my older brother uses another, simpler encryption method for his diary entries. He uses a substitution cipher where each letter in the plaintext is substituted by another letter from the alphabet. The distance between the plaintext letter and the encrypted letter is fixed. If we would define this fixed distance <em>d</em> to <em>5</em>, A would be replaced by F, B by G, C by H, ..., Y by D, Z by E.</p>
<p>With a fixed and known distance <em>d</em> the decryption would be somewhat simple. But my brother uses random distances for each of his diary entries. To decrypt his diary I have to guess the distance <em>d</em> for each entry. Thus, I use the well known phenomenon that the letter E is used more often in English words than other letters.  Can you write a program for me that calculates the distance <em>d</em> based on the fact that the most used letter in the encrypted text corresponds to the letter E in plaintext? Of course, I am interested in the decrypted text, too.</p>
<h3>Input</h3>
<p>The input consists of several test cases <em>c</em> that follow (<em>1 ¡Ü c ¡Ü 100</em>). Each test case is given in exactly one line containing one diary entry. Diary entries only use upper case letters (A-Z) and spaces. Each diary entry consists of at most <em>1000</em> encrypted letters (including spaces).</p>
<h3>Output</h3>
<p>For each test case, print one line containing the smallest possible distance <em>d</em> (<em>0 ¡Ü d ¡Ü 25</em>) and the decrypted text. If the decryption is not possible because there are multiple distances conforming to the rules above, print <strong>NOT POSSIBLE</strong> instead. Spaces are not encrypted.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
RD TQIJW GWTYMJWX INFWD JSYWNJX ZXJ F XNRUQJ JSHWDUYNTS YJHMSNVZJ
THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG
XVIDRE TFCCVXZRKV GIFXIRDDZEX TFEKVJK UVTIPGKZFE
XVIDRE TFCCVXZRKV GIFXIRDDZEX TFEKVJK

<strong>Output:</strong>
5 MY OLDER BROTHERS DIARY ENTRIES USE A SIMPLE ENCRYPTION TECHNIQUE
10 JXU GKYSA RHEMD VEN ZKCFI ELUH JXU BQPO TEW
17 GERMAN COLLEGIATE PROGRAMMING CONTEST DECRYPTION
NOT POSSIBLE
</pre>
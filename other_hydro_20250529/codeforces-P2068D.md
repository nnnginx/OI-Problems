## Description

<div><p>Morse code is a classical way to communicate over long distances, but there are some drawbacks that increase the transmission time of long messages. </p><p>In Morse code, each character in the alphabet is assigned a sequence of dots and dashes such that <span class="tex-font-style-bf">no sequence is a prefix of another</span>. To transmit a string of characters, the sequences corresponding to each character are sent in order. <span class="tex-font-style-bf">A dash takes twice as long to transmit as a dot.</span> </p><p>Your alphabet has $n$ characters, where the $i$-th character appears with frequency $f_i$ in your language. Your task is to design a Morse code encoding scheme, assigning a sequence of dots and dashes to each character, that minimizes the expected transmission time for a single character. In other words, you want to minimize $f_1t_1 + f_2t_2 + \cdots + f_nt_n$, where $t_i$ is the time required to transmit the sequence of dots and dashes assigned to the $i$-th character.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2\le n\le 200$) ！ the number of characters in the alphabet.</p><p>The second line contains $n$ real numbers $f_1$, $f_2$, $\ldots$, $f_n$ ($0 &lt; f_i &lt; 1$) ！ $f_i$ is the frequency of the $i$-th character. All values $f_1$, $f_2$, $\ldots$, $f_n$ are given with exactly four digits after the decimal point. The sum of all frequencies is exactly 1.</p></div><div class="output-specification"><p>Print $n$ lines, each containing one string consisting of dots $\texttt{.}$ and dashes $\texttt{-}$. The $i$-th line corresponds to the sequence of dots and dashes that you assign to the $i$-th character.</p><p>If there are multiple valid assignments with the minimum possible expected transmission time, any of them is considered correct.</p></div>

## Input

<p>The first line contains an integer $n$ ($2\le n\le 200$) ！ the number of characters in the alphabet.</p><p>The second line contains $n$ real numbers $f_1$, $f_2$, $\ldots$, $f_n$ ($0 &lt; f_i &lt; 1$) ！ $f_i$ is the frequency of the $i$-th character. All values $f_1$, $f_2$, $\ldots$, $f_n$ are given with exactly four digits after the decimal point. The sum of all frequencies is exactly 1.</p>

## Output

<p>Print $n$ lines, each containing one string consisting of dots $\texttt{.}$ and dashes $\texttt{-}$. The $i$-th line corresponds to the sequence of dots and dashes that you assign to the $i$-th character.</p><p>If there are multiple valid assignments with the minimum possible expected transmission time, any of them is considered correct.</p>





```input1|
3
0.3000 0.6000 0.1000
```




```input2|
3
0.3000 0.4500 0.2500
```




```output1
-.
.
--
```




```output2
..
-
.-
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, the alphabet contains three letters, say $a$, $b$, and $c$, with respective frequencies $0.3$, $0.6$, and $0.1$. In the optimal assignment, we assign $a$ to '$\texttt{-.}$', $b$ to '$\texttt{.}$', and $c$ to '$\texttt{--}$'. This gives an expected transmission time of $0.3 \cdot 3 + 0.6 \cdot 1 + 0.1 \cdot 4 = 1.9$ time units per character, which is optimal.</p><p>For comparison, the assignment $a\to$ '$\texttt{..}$', $b \to$ '$\texttt{-}$', $c \to$ '$\texttt{.-}$' has an expected transmission time of $0.3 \cdot 2 + 0.6 \cdot 2 + 0.1 \cdot 3 = 2.1$. The assignment $a \to$ '$\texttt{-}$', $b \to$ '$\texttt{.}$', $c \to$ '$\texttt{..}$' has a lower expected transmission time, but is invalid since '$\texttt{.}$' is a prefix of '$\texttt{..}$'.</p>

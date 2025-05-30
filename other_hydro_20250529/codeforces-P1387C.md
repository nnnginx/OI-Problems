## Description

<div><p>The Committee for Research on Binary Viruses discovered a method of replication for a large family of viruses whose genetic codes are sequences of zeros and ones. Each virus originates from a single gene; for simplicity genes are denoted by integers from $0$ to $G - 1$. At each moment in time a virus is a sequence of genes. When mutation occurs, one of the genes from the sequence is replaced by a certain sequence of genes, according to the mutation table. The virus stops mutating when it consists only of genes $0$ and $1$.</p><p>For instance, for the following mutation table: $$ 2 \to \langle 0\ 1 \rangle \\ 3 \to \langle 2\ 0\ 0\rangle\\ 3 \to \langle 1\ 3\rangle\\ 4 \to \langle 0\ 3\ 1\ 2\rangle\\ 5 \to \langle 2\ 1\rangle\\ 5 \to \langle 5\rangle $$ a virus that initially consisted of a single gene $4$, could have mutated as follows: $$ \langle 4 \rangle \to \langle \underline{0\ 3\ 1\ 2} \rangle \to \langle 0\ \underline{2\ 0\ 0}\ 1\ 2 \rangle \to \langle 0\ \underline{0\ 1}\ 0\ 0\ 1\ 2 \rangle \to \langle 0\ 0\ 1\ 0\ 0\ 1\ \underline{0\ 1} \rangle $$ or in another way: $$ \langle 4 \rangle \to \langle \underline{0\ 3\ 1\ 2} \rangle \to \langle 0\ \underline{1\ 3}\ 1\ 2 \rangle \to \langle 0\ 1\ 3\ 1\ \underline{0\ 1} \rangle \to \langle 0\ 1\ \underline{2\ 0\ 0}\ 1\ 0\ 1 \rangle \to \langle 0\ 1\ \underline{0\ 1}\ 0\ 0\ 1\ 0\ 1 \rangle $$</p><p>Viruses are detected by antibodies that identify the presence of specific continuous fragments of zeros and ones in the viruses' codes. For example, an antibody reacting to a fragment $\langle 0\ 0\ 1\ 0\ 0 \rangle$ will detect a virus $\langle 0\ 0\ 1\ 0\ 0\ 1\ 0\ 1 \rangle$, but it will not detect a virus $\langle 0\ 1\ 0\ 1\ 0\ 0\ 1\ 0\ 1 \rangle$.</p><p>For each gene from $2$ to $G-1$, the scientists are wondering whether a given set of antibodies is enough to detect all viruses that can emerge through mutations from this gene. If not, they want to know the length of the shortest virus that cannot be detected.</p><p>It may happen that sometimes scientists don't have any antibodies. Then of course no virus can be detected, so the scientists are only interested in the length of the shortest possible virus that can emerge from the gene mutations.</p></div><div class="input-specification"><p>The first line of the input will contain three integers $G$, $N$ and $M$ ($G &gt; 2$, $N \geq G - 2$, $M \geq 0$) specifying the number of genes, the number of rows in the mutation table, and the number of antibodies.</p><p>The following $N$ lines contain descriptions of rows of the mutation table; each line begins with two integers $a$ and $k$ ($2 \leq a &lt; G$, $k \geq 1$), followed by a sequence of $k$ integers $b_1, b_2, \ldots, b_k$ ($0 \leq b_i &lt; G$), that encode the row $$ a \to \langle b_1\ b_2\ \ldots\ b_k \rangle $$</p><p>The sum of all values $k$ does not exceed $100$. <span class="tex-font-style-bf">Every integer from $2$ to $G - 1$ appears in the table as $a$ at least once.</span></p><p>The next $M$ lines contain descriptions of the antibodies; each such line begins with an integer $\ell$ ($\ell \geq 1$), followed by a sequence of $\ell$ integers $c_1, c_2, \ldots, c_\ell$ ($0 \leq c_i \leq 1$), describing the antibody. The sum of all values $\ell$ does not exceed $50$.</p></div><div class="output-specification"><p>Your program needs to output exactly $G - 2$ lines, containing the answers for the subsequent genes from $2$ to $G - 1$.</p><p>If all viruses that can mutate from this single gene can be detected by the given set of antibodies, you need to print the word "<span class="tex-font-style-tt">YES</span>". You also need to print this if there are no viruses that could originate from this gene (it can happen when the sequences never stop mutating).</p><p>Otherwise you need to print the word "<span class="tex-font-style-tt">NO</span>", followed by an integer denoting the minimal length of the undetectable virus. You can assume that for all the prepared input data this value will be smaller than $2^{63}$.</p></div><div><h2>Scoring</h2><p>Subtasks: </p><ol> <li> (11 points) No antibodies ($M = 0$) </li><li> (14 points) $N = G - 2$ </li><li> (25 points) One antibody ($M = 1$) </li><li> (32 points) The sum of all values $\ell$ does not exceed $10$ </li><li> (18 points) No further constraints </li></ol></div>

## Input

<p>The first line of the input will contain three integers $G$, $N$ and $M$ ($G &gt; 2$, $N \geq G - 2$, $M \geq 0$) specifying the number of genes, the number of rows in the mutation table, and the number of antibodies.</p><p>The following $N$ lines contain descriptions of rows of the mutation table; each line begins with two integers $a$ and $k$ ($2 \leq a &lt; G$, $k \geq 1$), followed by a sequence of $k$ integers $b_1, b_2, \ldots, b_k$ ($0 \leq b_i &lt; G$), that encode the row $$ a \to \langle b_1\ b_2\ \ldots\ b_k \rangle $$</p><p>The sum of all values $k$ does not exceed $100$. <span class="tex-font-style-bf">Every integer from $2$ to $G - 1$ appears in the table as $a$ at least once.</span></p><p>The next $M$ lines contain descriptions of the antibodies; each such line begins with an integer $\ell$ ($\ell \geq 1$), followed by a sequence of $\ell$ integers $c_1, c_2, \ldots, c_\ell$ ($0 \leq c_i \leq 1$), describing the antibody. The sum of all values $\ell$ does not exceed $50$.</p>

## Output

<p>Your program needs to output exactly $G - 2$ lines, containing the answers for the subsequent genes from $2$ to $G - 1$.</p><p>If all viruses that can mutate from this single gene can be detected by the given set of antibodies, you need to print the word "<span class="tex-font-style-tt">YES</span>". You also need to print this if there are no viruses that could originate from this gene (it can happen when the sequences never stop mutating).</p><p>Otherwise you need to print the word "<span class="tex-font-style-tt">NO</span>", followed by an integer denoting the minimal length of the undetectable virus. You can assume that for all the prepared input data this value will be smaller than $2^{63}$.</p>

## Samples

```input1
6 6 2
2 2 0 1
3 3 2 0 0
3 2 1 3
4 4 0 3 1 2
5 2 2 1
5 1 5
2 1 1
5 0 0 1 0 0
```

```output1
NO 2
NO 4
NO 9
YES
```




<p align="justify">
You are hired by french NSA to break the RSA code used on the Pink
Card. The easiest way to do that is to factor the public modulus and
you have found the fastest algorithm to do that, except that you have
to solve a subproblem that can be modeled in the following way.
<br>
Let <img width="16" height="15" align="bottom" border="0" src="/content/ak15:SQDANCE1.png" alt="$ cal P$"><!-- MATH
$= {p_1,p_2,...,p_n}$
-->
<img width="118" height="32" align="middle" border="0" src="/content/ak15:SQDANCE2.png" alt="$ = {p_1,p_2,...,p_n}$"><!-- MATH
$S = {s_1,s_2,...,s_u}$
-->be
a set of prime numbers. If <img width="131" height="32" align="middle" border="0" src="/content/ak15:SQDANCE3.png" alt="$ S = {s_1,s_2,...,s_u}$"><!-- MATH
$T = {t_1,...,t_v}$
-->
and <img width="106" height="32" align="middle" border="0" src="/content/ak15:SQDANCE4.png" alt="$ T = {t_1,...,t_v}$"> are formed with elements
of <img width="16" height="15" align="bottom" border="0" src="/content/ak15:SQDANCE1.png" alt="$ cal P$">, then S*T will denote the quantity
<!-- MATH
begin{displaymath}
s_1*s_2*cdot cdot cdot *s_u*t_1*t_2*cdot cdot cdot *t_v.
end{displaymath}
-->
</p>
<img width="238" height="29" align="middle" border="0" src="/content/ak15:SQDANCE5.png" alt="$displaystyle s_1*s_2*cdot cdot cdot *s_u*t_1*t_2*cdot cdot cdot *t_v.$">
<p>
We call relation a set of two primes p,q, where p and q are distinct
elements of <img width="16" height="15" align="bottom" border="0" src="/content/ak15:SQDANCE1.png" alt="$ cal P$"><!-- MATH
$S_i = {p_i,q_i}$
-->.
You dispose of a collection of R
relations <img width="89" height="32" align="middle" border="0" src="/content/ak15:SQDANCE6.png" alt="$ S_i = {p_i,q_i}$"><!-- MATH
$S_{i_1}, S_{i_2}, ..., S_{i_k}$
-->
and you are interested in finding
sequences of these, <img width="103" height="30" align="middle" border="0" src="/content/ak15:SQDANCE7.png" alt="$ S_{i_1}, S_{i_2}, ..., S_{i_k}$">
such that
<!-- MATH
begin{displaymath}
S_{i_1}*S_{i_2}*cdot cdot cdot *S_{i_k}
end{displaymath}
-->
</p>
<img width="134" height="30" align="middle" border="0" src="/content/ak15:SQDANCE8.png" alt="$displaystyle S_{i_1}*S_{i_2}*cdot cdot cdot *S_{i_k}$">
<p>
is a perfect square.
</p><p>
The way you look for these squares is the following. The ultimate goal
is to count squares that appear in the process. Relations arrive one at
a time. You maintain a collection <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$"> of relations
that do not contain any square subproduct. This is easy: at first, <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$"> is empty. Then a relation arrives and <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$">
begins to grow.
Suppose a new relation <img width="43" height="32" align="middle" border="0" src="/content/ak15:SQDANCE10.png" alt="$ {p,q}$"> arrives. If no square
appears when adding <img width="43" height="32" align="middle" border="0" src="/content/ak15:SQDANCE10.png" alt="$ {p,q}$"> to <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$">,
then <img width="43" height="32" align="middle" border="0" src="/content/ak15:SQDANCE10.png" alt="$ {p,q}$"> is added to the collection.
Otherwise, a square is about to appear, we increase the number of
squares, but we do not store this relation, hence <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$">
keeps the desired property.
<br>
<!-- MATH
$S_1 = {2,3}$
-->Let us consider an example. First
arrives <img width="81" height="32" align="middle" border="0" src="/content/ak15:SQDANCE11.png" alt="$ S_1 = {2,3}$"> and we put it in <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$"><!-- MATH
$S_2 = {5,11},S_3 = {3,7}$
-->; then
arrives <img width="173" height="32" align="middle" border="0" src="/content/ak15:SQDANCE12.png" alt="$ S_2 = {5,11},S_3 = {3,7}$"> and they are
stored in <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$"><!-- MATH
$S_4 = {2,7}$
-->. Now
enters the relation <img width="81" height="32" align="middle" border="0" src="/content/ak15:SQDANCE13.png" alt="$ S_4 = {2,7}$">. This relation
could be used to form the
square:
<!-- MATH
begin{displaymath}
S_1*S_3*S_4 = (2*3)*(3*7)*(2*7) = (2*3*7)^2.
end{displaymath}
-->
</p>
<img width="365" height="36" align="middle" border="0" src="/content/ak15:SQDANCE14.png" alt="$displaystyle S_1*S_3*S_4 = (2*3)*(3*7)*(2*7) = (2*3*7)^2.$">
<p>
So we count 1 and do not store <img width="21" height="30" align="middle" border="0" src="/content/ak15:SQDANCE15.png" alt="$ S_4$"> in <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$"><!-- MATH
$S_5 = {5,11}$
-->. Now we consider <img width="89" height="32" align="middle" border="0" src="/content/ak15:SQDANCE16.png" alt="$ S_5 = {5,11}$"> that could make a square with <img width="21" height="30" align="middle" border="0" src="/content/ak15:SQDANCE17.png" alt="$ S_2$"><!-- MATH
$S_6 = {2,13}$
-->,
so we count 1 square more. Then <img width="89" height="32" align="middle" border="0" src="/content/ak15:SQDANCE18.png" alt="$ S_6 = {2,13}$"> is
put into <img width="13" height="14" align="bottom" border="0" src="/content/ak15:SQDANCE9.png" alt="$ cal C$"><!-- MATH
$S_7 = {7,13}$
-->. Now <img width="89" height="32" align="middle" border="0" src="/content/ak15:SQDANCE19.png" alt="$ S_7 = {7,13}$"><!-- MATH
$S_1*S_3*S_6*S_7$
--> could make
the square <img width="117" height="30" align="middle" border="0" src="/content/ak15:SQDANCE20.png" alt="$ S_1*S_3*S_6*S_7$">. Eventually, we get 3
squares.
<br>
</p>
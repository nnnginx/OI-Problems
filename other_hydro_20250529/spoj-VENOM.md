<p>
Sometimes you have to try fighting even though you know that your enemy is very powerful than you. Your hero with initial health H is about to fight against a venomous enemy who has a poisonous value of P. The enemy's poison deals i*P damage at it's ith attacking chance(i&gt;=1). The hero dies when his health becomes &lt;=0. After enemy's attack, if the hero survives, he heals himself with a health of A by using his skills. Then the enemy gets the chance again and the cycle continues till the hero dies. Find the survival time of the hero. You can safely assume that the hero is mortal.<br><br>

</p><p>Example Scenario:
</p><p>Initial Health(H) = 10, Poison (P) = 2, Heal value(A) = 1
</p><p>At time 1, enemy does 1*2 damage reducing the hero's health to 8
</p><p>At time 2, hero heals himself by 1 increasing his health to 9
</p><p>At time 3, enemy does 2*2 damage reducing the hero's health to 5
</p><p>At time 4, hero heals himself by 1 increasing his health to 6
</p><p>At time 5, enemy does 3*2 damage and kill the hero.
</p><p>The hero survived 5 units of time.<br><br>

</p><p><b>Input:</b>
</p><p>The first line consists of an integer t, the number of test cases. For each test case there is a line with 3 integers H, P and A.<br><br>

</p><p><b>Output:</b>
</p><p>For each test case, find the survival time of the hero.<br><br>

</p><p><b>Input Constraints:</b>
</p><p>1&lt;=t&lt;=10^6
</p><p>1&lt;=H&lt;=10^6
</p><p>1&lt;=P&lt;=10^6
</p><p>0&lt;=A&lt;P<br><br>

</p><p><b>Sample Input:</b>
</p><p>3
</p><p>3 7 2
</p><p>81 4 1
</p><p>87 8 4<br><br>

</p><p><b>Sample Output:</b>
</p><p>1
</p><p>13
</p><p>9<br><br>
</p>
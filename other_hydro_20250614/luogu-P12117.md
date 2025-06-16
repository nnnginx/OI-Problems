## Ã‚ƒø√Ë ˆ
\textit{Pr®¶f®¶rence} is a card game which is very popular in Eastern Europe. It is usually played with a 32-card deck, which consists of pip cards from 7 to 10, Jack, Queen, King, and Ace in each of the four suits: Spades, Clubs, Diamonds, and Hearts. In each round of the game, three players receive ten cards each, and two cards are left on the table as a talon. Then, a phase of auction happens, where players make their bids, which are obligations to take at least a certain number of tricks. A special case of a bid is a so-called \textit{mis®®re}, which is an obligation to take no tricks regardless of other players' moves.

In this task, we will consider a special modification of pr®¶f®¶rence which is played with a modified deck containing $A\cdot B$ cards, where $A$ is a number of suits, and $B$ is the number of ranks in each suit. For example, the standard 32-card deck for the pr®¶f®¶rence game has $A = 4$ suits and $B = 8$ ranks. For convenience, we'll number the suits from $1$ to $A$, and the ranks from $1$ to $B$.

You need to solve a puzzle about this modification of pr®¶f®¶rence. In this modification, we'll say that a mis®®re is \textit{guaranteed} if for every suit, after we order the cards belonging to this suit in your hand by their rank as $b_1 < b_2 < \cdots < b_k$ (where $k$ is the number of cards of the suit in your hand), the following condition is satisfied: $b_i \le 2i - 1$ for all $i$ from $1$ to $k$. If you don't have any cards of the suit ($k = 0$), the condition is trivially satisfied.

You have $n$ cards in your hand, and you will be allowed to choose any $x$ cards you don't have and add them to your hand. Then, you must select any $x$ of your $n + x$ cards and drop them, leaving some $n$ cards in your hand. Your task is to find the smallest possible $x$ such that you can transform your hand to a guaranteed mis®®re.

```input1
2
4 2 6
1 1
1 2
1 6
2 3
2 4 5
3 4
2 4
```

```output1
1
2
```


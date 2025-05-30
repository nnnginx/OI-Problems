## Description

Farmer John is helping to turn his large field into a ski course for the upcoming winter Moolympics. The field has dimensions $M \times N$ ($1 \leq M,N \leq 100$), and its intended final composition is described by an $M \times N$ grid of characters like this:

```
RSRSSS
RSRSSS
RSRSSS
```

Each character describes how the snow in a unit square of the field should be groomed: either `R` for rough or `S` for smooth (the Moolympics organizers think that a course is more interesting if it has a mixture of rough and smooth patches).

To build the desired course, Farmer John plans to modify his tractor so that it can stamp any $B \times B$ patch of the field ($B \leq M$, $B \leq N$) with either entirely smooth snow or entirely rough snow. Since it takes a long time to reset the tractor between each of these stamps, FJ wants to make $B$ as large as possible. With $B = 1$, he can clearly create the desired ski course by stamping each individual square with either `R` or `S`, as intended. However, for larger values of $B$, it may no longer be possible to create the desired course design. Every unit square of the course must at some point be stamped by FJ's tractor; it cannot be left in its default state.

Please help FJ determine the largest possible value of $B$ he can successfully use.

## Input

* Line $1$: Two space-separated integers $M$ and $N$.

* Lines $2 \sim M+1$: $M$ lines of exactly $N$ characters (each `R` or `S`),  describing the desired ski course design.

## Output

* Line 1: The maximum value of $B$ Farmer John can use to create the desired course pattern.

```input1
3 6
RSRSSS
RSRSSS
RSRSSS
```

```output1
3
```

## Sample Explanation

FJ can stamp a rough patch spanning columns $1 \sim 3$, followed by a smooth patch spanning columns $2 \sim 4$, then a rough patch spanning columns $3 \sim 5$, and finally a smooth patch spanning columns $4 \sim 6$.
## Statement

Farmer John's cows are on a road trip! The odometer on their car displays an integer mileage value, starting at $X$ miles at the beginning of their trip and ending at $Y$ miles at the end of their trip. Whenever the odometer displays an 'interesting' number (including at the start and end of the trip) the cows will moo. A number is 'interesting' if when you look at all its digits except for leading zeros, at least half of these should be the same. For example, the numbers $3223$ and $110$ are interesting, while the numbers $97791$ and $123$ are not. Help FJ count how many times the cows will moo during the trip. 

## Input Format

Line $1$: The first line will contain two integers, $X$ and $Y$, separated by a space. 

## Output Format

Line $1$: A single integer containing how many times the cows will moo during the trip. 

```input1
110 133 

```
```output1
14 
```

INPUT DETAILS: 

The trip starts with the odometer at $110$ and ends at $133$.

OUTPUT DETAILS:

The cows moo when the odometer reads $110$, $111$, $112$, $113$, $114$, $115$, $116$, $117$, $118$, $119$, $121$, $122$, $131$, and $133$. 

## Constraints

$100 \le X \le Y \le 10^{18}$

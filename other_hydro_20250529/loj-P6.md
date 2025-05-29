## Description

## Work in Progress
This is a template problem for interactive problems.

The system will generate $n$ random numbers $a_i$ and your task is to guess the value of those $n$ values through ways like enumeration, binary search answers and guessing. However, your score will be determined by how many times you guessed.

### How to Interact

For C++ users, you can use the library given to interact with the system. For users of other languages, you can use standard input/output to easily interact with the system with the friendly interface provided.

#### Interact without Library

To better demonstrate the usage of interactive problems, three (3) kinds of operations are designed:

1. `get_num`: Get the count of values, $n$. No parameters required for this operation.

2. `guess`: Guess a number. Two (2) parameters are required: the index of number being guessed, starting from zero, and the value of that number. The return value will be `-1` if your guess is less than the actual value, `1` if larger than that, and `0` if correctly guessed.

3. `submit`: Submit your answer. This operation requires $n$ parameters, correspondingly represent the $n$ numbers. No return value for this operation.

Please write to the standard output with the format below if you want to perform an operation.

```plain
<Operation Name> <Parameter 1> <Parameter 2> ... <Parameter n>
```

An line break **must** be there following your request and redundant white characters will be ignored.




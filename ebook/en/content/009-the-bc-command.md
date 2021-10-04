# The `bc` command


The `bc` command is used for command line calculator. It is used for basic calculations and arithmetic operations.

### Examples of uses:


1 . Arithmetic:

```
Input : $ echo "11+5" | bc
Output : 16
```
2 . Increment:
- var –++ : Post increment operator, result of the variable is used first and then variable is incremented.
- – ++var : Pre increment operator, variable is increased first and then result of variable is stored.

```
Input: $ echo "var=3;++var" | bc
Output: 4
```
3 . Decrement:
- var – – : Post decrement operator, result of the variable is used first and then variable is decremented.
- – – var : Pre decrement operator, variable is decreased first and then result of variable is stored.

```
Input: $ echo "var=3;--var" | bc
Output: 2
```
4 . Assignment:
- var = value : Assign the value to the variable
- var += value : similar to var = var + value
- var -= value : similar to var = var – value
- var *= value : similar to var = var * value
- var /= value : similar to var = var / value
- var ^= value : similar to var = var ^ value
- var %= value : similar to var = var % value

```
Input: $ echo "var=4;var" | bc
Output: 4
```
5 . Comparison or Relational:
- If the comparison is true, then result is 1. Otherwise(false), returns 0
- expr1<expr2 : Result is 1, if expr1 is strictly less than expr2.
- expr1<=expr2 : Result is 1, if expr1 is less than or equal to expr2.
- expr1>expr2 : Result is 1, if expr1 is strictly greater than expr2.
- expr1>=expr2 : Result is 1, if expr1 is greater than or equal to expr2.
- expr1==expr2 : Result is 1, if expr1 is equal to expr2.
- expr1!=expr2 : Result is 1, if expr1 is not equal to expr2.

```
Input: $ echo "6<4" | bc
Output: 0
```
```
Input: $ echo "2==2" | bc
Output: 1
```
6 . Logical or Boolean:

- expr1 && expr2 : Result is 1, if both expressions are non-zero.
- expr1 || expr2 : Result is 1, if either expression is non-zero.
- ! expr : Result is 1, if expr is 0.

```
Input: $ echo "! 1" | bc
Output: 0

Input: $ echo "10 && 5" | bc
Output: 1
```


### Syntax:

```
bc [ -hlwsqv ] [long-options] [ file ... ] 
```

### Additional Flags and their Functionalities:

|**Short Flag**   |**Long Flag**   |**Description**   |
|:---|:---|:---|
|`-h`|<center>-help </center>|Help. More information.|
|`-i`|<center>-interactive</center>|Force Interactive mode.|
|`-l`|<center>-mathlib</center>|Mathlib. Standard math library|
|`-w`|<center>-warn</center>|Give warning for POSIC bc.|
|`-s`|<center>-standard</center>|Process exactly the POSIX bc language.|
|`-q`|<center>-quiet </center>|Does not print the normal GNU welcome.|
|`-v`|<center>-version</center>|Version and copyright information.|

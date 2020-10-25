## Introduction to Algorithms
---
### What is Algorithm?
> An Algorithm is a step by step process for solving a computational problem
---
### Difference between Algorithm and Program
| Algorithm | Program |
|---|---|
| Design Phase | Implementation Phase |
| Domain Knowledge expert | Programmer |
| Pseudo Code | Programming Language |
| Not Dependent on Harware | Dependent on Harware and OS |
---
| Priori Analysis | Posteriori Testing |
|---|---|
| Algorithm | Program |
| Independent on Language | Language Dependent |
| Hardware Independent | Hardware Dependent |
| Time & Function | Watch time & Bytes |

---

### Characteristics of an Algorithm

1. It needs zero or more Inputs.
1. An Algorithm should produce atleast one output otherwise it is useless.
2. It should be very definite means it should be very clear not confusing.
3. Finiteness - Finite Duration and controlled.
4. Effectiveness

---

### How to write an Algorithm

```javascript
    Algorithm swap(a, b) {
        temp = a ---- 1 unit of time
        a = b    ---- 1 unit of time
        b = temp ---- 1 unit of time
    }
    ___________________________________
               f(n) = 3 -> contant time
               O(1)
```

#### Space analysis
```
a    ---- 1 word
b    ---- 1 word
temp ---- 1 word
________________
   s(n) = 3 words O(1)
```

> Consider an algorithm for swapping number. Here we are considering C language kind of syntax for algorithm it can be any kind of pseudo code.

> Let us consider for execution of every instrcution it is taking one unit of time and one word for storing one variable because this is a pseudo code Algorithm for design analysis.

### How to analyse an Algorithm
1. Time
2. Space
3. Network Consumption
4. Power Consumption
5. Registers Usuage

### Frequency count method

```javascript
    Algorithm sum(A, n) {
        s = 0;                  ---- 1 unit of time
        for(i = 0; i < n; i ++) ---- (n + 1) unit of time
        {
            s = s + A[i];       ---- n unit of time
        }
        return s;               ---- 1 unit of time
    }
    _________________________________________________
                f(n) = 1 + (n + 1) + n + 1 = (2n + 3)

    > i < n condition checks for n + 1 times
    > Inside for loop block s = s + A[i] executes for n times
```
> Consider above sum function which will take arguments an array A and n will be the length of the array. Lets consider a [8, 3, 9, 7, 2] where length n will be 5. And FOR loop condition i < n will be tested for n + 1 times and in the last interation condition fails and loop executes for n times. i = 0 will be one time assignment.
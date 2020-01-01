---
title: "Complexity Analysis of Algorithms:"
metaTitle: "This is the title tag of this page"
metaDescription: "This is the meta description"
---

## Complexity Analysis of Algorithms:

1. Asymptotic Analysis
2. Worst, Average And Best Cases 
3. Asymptotic Notations 
4. Analysis Of Loops 
5. Analysis Of Recursion: Solving Recurrences 
6. Amortized Analysis 
7. Space Complexity




### 1. Analysis Of Loops

1. **O(1):**Time complexity of a function (or set of statements) is considered
as O(1) if it doesn’t contain loop, recursion and call to any other non-constant
time function. For example, swap() function has O(1) time complexity.

```javascript
   void swap (int x, int y) 
    {
    int tmp = x; x = y; y = tmp; 
    }
```
Note that the loop/code that runs a constant number of times is also considered
as O(1).

2. **O(n):**Time Complexity of a loop is considered as O(n) if the loop
variables is

incremented/decremented by a constant amount. For example following functions
have O(n) time complexity.

EX : Here c is a positive integer constant 

a)

```javascript
   for (int i = 1; i <= n; i += c)
    {
      // some O(1) expressions 
    }
```

b) 
```javascript
   for (int i = n; i > 0; i -= c)
    { 
        // some O(1) expressions 
    }
```

3. **O(nc):**Time complexity of nested loops is equal to the number of times
the innermost statement is executed. For example, the following sample loops have O(n2) time complexity.

A)
```javascript
    for (int i = 1; i <=n; i += c) 
    {
       for (int j = 1; j <=n; j += c)
       { // some O(1) expressions }
    } 
```

B) 
```javascript

    for (int i = n; i > 0; i -= c) 
    {
       for (int j = i+1; j <=n; j += c) 
         { // some O(1) expressions }
    }
```

4. **O(logn):** Time Complexity of a loop is considered as O(logn) if the loop
variables is **divided/multiplied** by a constant amount.

a. 
```javascript
    for (int i = 1; i <=n; i *= c) 
      {// some O(1) expressions }
``` 

b.
```javascript
   for (int i = n; i > 0; i /= c)
     { // some O(1) expressions }``` 
```
For example Binary Search has O(logn) time complexity.

5. **O(log logn):** Time Complexity of a loop is considered as O(log (logn)) if
the loop variables are **reduced/increasedexponentially** by a constant amount.

Here c is a constant greater than 1
```javascript
    for (int i = 2; i <=n; i = pow(i, c))
     {// some O(1) expressions }
```

Here fun is sqrt or cube root or any other constant root

B)
```javascript
    for (int i = n; i > 0; i = fun(i))
     {// some O(1) expressions }
```

**How to combine time complexities of consecutive loops? **When there are
consecutive loops, we calculate time complexity as sum of time complexities of
individual loops.

```javascript
    for (int i = 1; i <=m; i += c)
       {// some O(1) expressions } 
    for (int i = 1; i <=n; i += c) 
        { // some O(1) expressions }
```

* Time complexity of above code is O(m) + O(n) which is O(m+n)
* If m == n, the time complexity becomes O(2n) which is O(n).


**Analysis Of Recursive Algorithms: Solving Recurrences**Many algorithms are
recursive in nature. When we analyze them, we get a recurrence relation for time
complexity. We get running time on an input of size n as a function of n and the
running time on inputs of smaller sizes.

For example in Merge Sort, to sort a given array, we divide it in two halves and
recursively repeat the process for the two halves. Finally, we merge the
results. Time complexity of Merge Sort can be written as T(n) = 2T(n/2) + n.
There are many other recursive algorithms like Binary Search, Tower of Hanoi,
etc.

There are mainly three ways for solving recurrences.

**1) Substitution Method:**

**2) Recurrence Tree Method:**

**3) Master Theorem:**

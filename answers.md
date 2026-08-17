# CMPS 2200 Recitation 02
## Answers

**Name:**_________________________
**Name:**_________________________


Place all written answers from `recitation-02.md` here for easier grading.

- **4)** (3 points) Now, derive the asymptotic behavior of $W(n)$ using $f(n) = 1$, $f(n) = n$, and $f(n) = n^2$  with $a=2$ and $b=2$. Then, generate actual values for $W(n)$ for your code and confirm that the trends match your derivations.

- **5)** (4 points) Now that you have a nice way to empirically 
  generate values of $W(n)$, we can look at the relationship 
  between $a$, $b$, and $f(n)$. If $f(n) = n^c$, we can derive 
  a very nice result.
  
  The Master Method gives an easy formula for solving general 
  recurrences of the form: 

    $$T(n) = aT(n/b) + n^c$$

  Its three cases correspond to the relationship between $\log_b a$ 
  and $c$. Derive the asymptotic behavior of $T(n)$ by solving its 
  general recursion tree for each of the three cases. Show your 
  recursion tree and derivations from it.

  1. $\log_b a < c$

  2. $\log_b a = c$

  3. $\log_b a > c$ 

- **6)** (2 points) $W(n)$ is meant to represent the running time of
  some recursive algorithm. Assume that we always have enough processors for every generated subproblem. Implement the function `span_calc` to compute the empirical span, where the work of the algorithm is given by $W(n)$ and the span of the combine step is equal to the work of the combine step. Test this code by completing the test cases in `test_main.py::test_span`.

- **7)** (3 points) Derive the asymptotic expressions for the span of the recurrences you used in problem 4 above. Confirm that everything matches up as it should. 
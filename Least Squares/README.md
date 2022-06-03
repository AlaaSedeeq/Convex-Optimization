### Least Squares (Linear Regression)

- Given:
    - $A^{m,n}$
    - $b∈R^m$
    - $m > n$<br><br>

- This system has a solution if $b ∈ Span(A)$, the column space of $A$, but normally this is not the case and we can only find an approximate solution.<br><br>
- $AX = b$ has no solution, because we have $m > n$ (too many equations), or the n columns of $A$ spans a small part of $R^m$, or $e = b-AX \neq 0$, if e is zero, then $X$ is the exact solution.<br><br>

- A general approach is to:
    - Find the prjection of $b$ onto the column space of $A$ which minimizes this errror e
    - Then, solve $A X^{*} = P$ instead of $AX = b$<br><br>

- This can be formulaize as :
    - $\sum_{i=1}^{m} (a_{i}^Tx - b_{i})$, also known as the $L_{2}$-norm squared $||Ax−b||_{2}$<br><br>
- So the problem now is:
    - minimize $\quad$$||Ax−b||_{2}^2$

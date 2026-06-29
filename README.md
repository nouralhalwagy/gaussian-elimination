# Gaussian Elimination Solver

A Gaussian Elimination algorithm implemented from scratch using NumPy. Supports both singular and non-singular matrices, and detects whether a system has no solution or infinite solutions.

---

## How to Use

There are **two ways** to input your matrix:

---

### Way 1: Separate A and B matrices

```python
A = np.array([[2, -1, 1],
              [2,  2, 4],
              [4,  1, 0]])

B = np.array([[1],
              [-2],
              [1]])

Gaussian_Elimination(A, B)
```

---

### Way 2: Linear System of Equations

If you have a linear system like:

```
2a -  b +  c =  1
2a + 2b + 4c = -2
4a +  b + 0c =  1
```

> ⚠️ **Important:** Only enter the **coefficients and the result**, not the full equation. Writing the full equation will cause an error.

Your input should be:

```
2   -1   1   1
2    2   4   -2
4    1   0   1
```

Where each row follows the format:
```
coefficient1   coefficient2   coefficient3   result
```

---

## Output

- If the system has a **unique solution** → returns `x, y, z` values
- If the matrix is **singular** → prints `"Matrix has infinite Solutions"` or `"Matrix has no Solution"`

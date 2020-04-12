# Linear algebra

## Problem

Use back-substitution to solve the system.

$-x + y - z = 0$

$5y + z = 3$

$\frac{1}{3}z = 0$

## Solution

$$
\begin{bmatrix}
-1 & 1 & -1 & 0 \\
0 & 5 & 1 & 3 \\
0 & 0 & \frac{1}{3} & 0
\end{bmatrix}
$$

$3 \cdot R_3 \rightarrow R_3$

$$
\begin{bmatrix}
-1 & 1 & -1 & 0 \\
0 & 5 & 1 & 3 \\
0 & 0 & 1 & 0
\end{bmatrix}
$$


$R_2 - R_3 \rightarrow R_3$

$$
\begin{bmatrix}
-1 & 1 & -1 & 0 \\
0 & 5 & 0 & 3 \\
0 & 0 & 1 & 0
\end{bmatrix}
$$

$R_1 + R_3 \rightarrow R_1$

$$
\begin{bmatrix}
-1 & 1 & 0 & 0 \\
0 & 5 & 0 & 3 \\
0 & 0 & 1 & 0
\end{bmatrix}
$$

$\frac{R_2}{5} \rightarrow R_2$

$$
\begin{bmatrix}
-1 & 1 & 0 & 0 \\
0 & 1 & 0 & \frac{3}{5} \\
0 & 0 & 1 & 0
\end{bmatrix}
$$

$R_1 - R_2 \rightarrow R_1$

$$
\begin{bmatrix}
-1 & 0 & 0 & -\frac{3}{5} \\
0 & 1 & 0 & \frac{3}{5} \\
0 & 0 & 1 & 0
\end{bmatrix}
$$

$R_1 \cdot (-1) \rightarrow R_1$

$$
\begin{bmatrix}
1 & 0 & 0 & \frac{3}{5} \\
0 & 1 & 0 & \frac{3}{5} \\
0 & 0 & 1 & 0
\end{bmatrix}
$$

$\boxed{ (x, y, z) = \left( \frac{3}{5}, \frac{3}{5}, 0 \right) }$

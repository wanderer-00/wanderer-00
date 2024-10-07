$$
\begin{aligned}
d_{i, j} &\leftarrow d_{i, j} + 1 \\
d_{i, y + 1} &\leftarrow d_{i, y + 1} - 1 \\
d_{x + 1, j} &\leftarrow d_{x + 1, j} - 1 \\
d_{x + 1, y + 1} &\leftarrow d_{x + 1, y + 1} + 1
\end{aligned}
$$

```mermaid
graph TD;
  A-->B;
  A-->C;
  B-->D;
  C-->D;
  A-->X;
  B-->X;
  C-->X;
  D-->X;
```

```mermaid
pie
  Круговая диаграма
  "A" : 42.96
  "B" : 50.05
  "C" : 10.01
  "D" : 5
```

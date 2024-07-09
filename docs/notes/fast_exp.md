# exp 的快速求解

## 神秘数字

$$
\left\{\begin{matrix}
y=e^x \\
x=(-1)^{s_x} \cdot (1+m_x) \cdot 2^{e_x-bias_x} \\
y=(-1)^{s_y} \cdot (1+m_y) \cdot 2^{e_y-bias_y}
\end{matrix}\right.
$$
等价为：
$$
(-1)^{s_y} \cdot (1+m_y) \cdot 2^{e_y-bias_y} = e^{(-1)^{s_x} \cdot (1+m_x) \cdot 2^{e_x-bias_x}}
$$
i.e.，求解其中的 $s_y$，$m_y$  和 $e_y$

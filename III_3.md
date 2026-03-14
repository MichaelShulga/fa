# Часть III, Задача 3

Очевидно, что $A_n = (A_1)^n$, $\forall T, S \in \mathcal{L}(\ell_2) \implies (TS)^* = S^* T^*$

$((y, TSx) = (T^* y, Sx) = (S^* T^* y, x))$

$\implies A_n^* = ((A_1)^n)^* = ((A_1)^*)^n$

Пусть $B(x_1, \dots) = (0, x_1, \dots)$. Тогда $(y, A_1 x) = \sum\limits_{k \in \mathbb{N}} \overline{y(k)} (Ax)(k) =$

$= \sum\limits_{k \in \mathbb{N}} \overline{y(k)} x(k+1) = \sum\limits_{k \in \mathbb{N}} \overline{(By)(k+1)} x(k+1) = ((By)(1) = 0) = \sum\limits_{k \in \mathbb{N}} \overline{(By)(k)} x(k) \implies \boxed{B = A_1^*} \implies A_n^* = B^n \cdot B^n(x_1, \dots) = (0, \dots, 0, x_1, \dots)$

$$\|A_n x\|_2^2 = \sum_{k=n+1}^{\infty} |x(k)|^2 \to 0, n \to \infty \implies \forall x \in \ell_2 \implies A_n x \to 0, n \to \infty$$

Пусть $e_1 = (1, 0, \dots)$. Тогда $\|(B_n - B_m) e_1\|_2 = 2$ при $n \neq m \implies$

$B_n e_1$ расходится $\implies$ поточечной сходимости нет

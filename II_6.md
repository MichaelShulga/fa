# Часть II, Задача 6

Пусть $X$ - конечномерное линейное нормированное пространство

Понятно, что для $f \in X^*$

и $x_n \to x \implies f(x_n) \to f(x)$. То есть $x_n \xrightarrow{w} x$

Пусть $\{e_k\}_{k=1}^m$ - базис в $X \implies$ рассмотрим функционалы

$\pi_k: \quad \pi_k(e_j) = \delta_{kj} \implies$ если $x_n \xrightarrow{w} x$, то $\forall k \in \overline{1, m} \ \pi_k(x_n) \to \pi_k(x) \implies$

$$\|x_n - x\| = \left\|\sum_{k=1}^m (\pi_k(x_n) - \pi_k(x)) e_k\right\| \leq \sum_{k=1}^m |\pi_k(x_n) - \pi_k(x)| \|e_k\| \to 0 \implies x_n \to x$$

Получим: $\boxed{x_n \to x \iff x_n \xrightarrow{w} x}$

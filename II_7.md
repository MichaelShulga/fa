# Часть II, Задача 7

Пусть $\exists \ \{x_n\}_{n \in \mathbb{N}} \subseteq \ell_1 : x_n \xrightarrow{w} 0$, $x_n \not\to 0$

$\implies \exists \ \varepsilon > 0$ т.ч. $\forall n_0 \in \mathbb{N} \ \exists n : \|x_n\|_1 > \varepsilon \implies$

Перейдя к подпоследовательности будем считать, что $\forall n \in \mathbb{N} \ \|x_n\|_1 > \varepsilon$

Без ограничения общности $\varepsilon = 1$, иначе перейдем к последовательности $\left\{\frac{x_n}{\varepsilon}\right\}_{n \in \mathbb{N}}$

Теперь заметим, что из того, что $x_n \xrightarrow{w} 0$ следует $\forall k \in \mathbb{N} \ x_n(k) \to 0 \implies$

Найдем $m_1$ такое, что $\sum\limits_{k=1}^{m_1} |x_1(k)| \geq \frac{2}{3} \|x_1\|_1$. Найдется такое $n_2$, что $\forall n > n_2 \ \sum\limits_{k=1}^{m_1} |x_n(k)| < \frac{1}{3} \implies$

Найдем $m_2$ такое, что $\sum\limits_{k=m_1+1}^{m_2} |x_{n_2}(k)| \geq \frac{2}{3} \|x_{n_2}\|_1$. Найдется такое $n_3$, что $\forall n > n_3 \ \sum\limits_{k=1}^{m_2} |x_n(k)| < \frac{1}{3} \implies \dots$

Опишем индуктивную процедуру:

Пусть построены $n_j$ и $m_j$ так, что $\forall n > n_j \ \sum\limits_{k=1}^{m_j} |x_n(k)| < \frac{1}{3} \implies$

Найдем $m_{j+1}$ так, что $\sum\limits_{k=m_j+1}^{m_{j+1}} |x_{n_j}(k)| \geq \frac{2}{3} \|x_{n_j}\|_1$. Найдем $n_{j+1}$ такое, что $\forall n > n_{j+1} \ \sum\limits_{k=1}^{m_{j+1}} |x_n(k)| < \frac{1}{3} \implies$

По $m_j$ и $n_j$ построим $m_{j+1}$ и $n_{j+1} \implies$ доопределив $n_1 = 1$, $m_0 = 0$ имеем последовательности $\{n_j\}_{j \in \mathbb{N}}$ и $\{m_j\}_{j \in \mathbb{N}_0}$

Определим $y \in c_0$ так: $y(k) = \text{sgn } x_{n_j}(k)$, $k \in (m_{j-1}, m_j]$

$\bigcup\limits_{j \in \mathbb{N}} (m_{j-1}, m_j] \cap \mathbb{N} = \mathbb{N} \implies y$ опр. корректно

Теперь $\varphi(x) = \langle y, x \rangle \implies$

$$\varphi(x_{n_j}) = \sum_{k=m_{j-1}+1}^{m_j} |x_{n_j}(k)| + \sum_{k \in (m_{j-1}, m_j]^c} x_{n_j}(k) y(k) \geq \frac{2}{3} \|x_{n_j}\|_1 - \frac{1}{3} \|x_{n_j}\|_1 = \frac{1}{3} \|x_{n_j}\|_1 > \frac{1}{3} > 0 \implies$$

$\varphi(x_{n_j}) \not\to 0 \implies x_n \xrightarrow{w} 0 \implies$ противоречие $\implies$ такой $\{x_n\}_{n \in \mathbb{N}}$ нет

Тогда получаем $x_n \to 0 \iff x_n \xrightarrow{w} 0$

Теперь заметим, что $x_n \to x \iff x_n - x \to 0 \iff x_n - x \xrightarrow{w} 0 \iff x_n \xrightarrow{w} x \implies$

Наконец: $\boxed{x_n \to x \iff x_n \xrightarrow{w} x}$

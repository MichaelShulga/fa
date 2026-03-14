# Часть II, Задача 3

$$f_n(x) = \sin nx$$

Известно, что $\left\{\frac{1}{\sqrt{2\pi}} e^{ikx}\right\}_{k \in \mathbb{Z}}$ - ортобазис в $L_2([-\pi, \pi])$

Пусть $\varphi$ - непрерывный функционал на $L_2([-\pi, \pi])$

Тогда $\varphi(f) = (y, f)$. Известно, что $y = \sum\limits_{k \in \mathbb{Z}} a_k e^{ikx}$

$$\sin nx = \frac{e^{inx} - e^{-inx}}{2i} \implies (y, f_n) = \left(a_n e^{inx} + a_{-n} e^{-inx}, \frac{e^{inx} - e^{-inx}}{2i}\right) = \frac{\overline{a_n} - \overline{a_{-n}}}{2i} \to 0, n \to \infty$$

$\implies f_n \xrightarrow{w} 0$

Сильной сходимости нет: $(f_n \perp f_m \implies)$

$$\|f_n - f_m\|^2 = \|f_n\|^2 + \|f_m\|^2 = 4\pi \implies$$

$\{f_n\}$ не фундаментальна $\implies$ не сходится сильно

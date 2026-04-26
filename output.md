# Часть I, Задача 1

Заметим, что всякий вектор из $\ell_q$ задает непрерывный функционал на
$\ell_p$, где $\frac{1}{p} + \frac{1}{q} = 1$,
$1 \leq p, q \leq +\infty$
$$
f_y(x) = (y, x) = \sum_{k=1}^{\infty} x(k)y(k), \text{ причем}
$$
$$|f_y(x)| \leq \|x\|_p \|y\|_q < +\infty \implies \|f_y\|_{\ell_p^*} \leq \|y\|_q
$$
*(неравенство Гёльдера)*

Теперь рассмотрим произвольный непрерывный функционал на $\ell_p$,
$1 < p < +\infty$
$$
f(x) = \sum_{k \in \mathbb{N}} x(k)f(e_k)
$$
Пусть $y_f \in \mathbb{C}^{\mathbb{N}}$, $y_f(k) = f(e_k)$
$$
\left(z \in \mathbb{C} \implies \text{sgn } z = \begin{cases} \frac{z}{|z|}, & z \neq 0 \\ 0, & z = 0 \end{cases}\right)
$$
Пусть $x_f^n \in \mathbb{C}^{\mathbb{N}}$
$$
\begin{cases} x_f^n(k) = \text{sgn } y_f(k) \cdot |y_f(k)|^{q-1}, & k \leq n \\ x_f^n(k) = 0, & k > n \end{cases}
$$
Очевидно, что $x_f^n \in c_0 \subset \ell_p$
$$
\implies \langle y_f, x_f^n \rangle = \sum_{k=1}^{n} |y_f^k| \leq \|f\| \cdot \|x_f^n\|_p \implies \|f\| \geq \lim_{n \to \infty} \frac{\sum_{k=1}^{n} |y_f(k)|^q}{\left(\sum_{k=1}^{n} |y_f(k)|^{p(q-1)}\right)^{1/p}}
$$
Заметим, что
$\frac{1}{p} + \frac{1}{q} = 1 \implies \frac{q}{p} = q-1 \implies q = p(q-1) \implies$
$$
\|f\| \geq \lim_{n \to \infty} \left(\sum_{k=1}^{n} |y_f(k)|^q\right)^{1-\frac{1}{p}} = \lim_{n \to \infty} \left(\sum_{k=1}^{n} |y_f(k)|^q\right)^{\frac{1}{q}} = \|y_f\|_q \implies
$$
$$y_f \in \ell_q \text{ и } \|f\| \geq \|y_f\|
$$
------------------------------------------------------------------------

## Случай p = 1

Теперь пусть $p = 1$. Тогда снова в силу непрерывности функционала $f$:
$$
f(x) = \sum_{k=1}^{\infty} x(k)f(e_k) \text{ и } y_f(k) = f(e_k)
$$
Тогда пусть $x_f^n = \text{sgn } y_f(k) \cdot e_k$
$$
\|x_f^n\|_1 = 1 \implies
$$
$$\|f\| \geq |\langle y_f, x_f^n \rangle| = \text{sgn } y_f(k) \cdot y_f(k) = |y_f(k)| \implies
$$
$$\|f\| \geq \sup |y_f(k)| = \|y_f\|_{\infty}
$$
$$\implies y_f \in \ell_{\infty} \text{ и } \|f\| \geq \|y_f\|_{\infty}
$$
------------------------------------------------------------------------

## Изоморфизм $\ell_p^* \cong \ell_q$

Для $1 \leq p, q$;
$\begin{cases} p < +\infty \\ q < +\infty \end{cases}$,
$\frac{1}{p} + \frac{1}{q} = 1$ рассмотрим отображения
$$
\varphi: y \mapsto f_y \quad (\varphi: \ell_q \to \ell_p^*)
$$
$$\psi: f \mapsto y_f \quad (\psi: \ell_p^* \to \ell_q)
$$
Заметим, что $\psi \circ \varphi = \text{Id}_{\ell_q}$, $\varphi$ и
$\psi$ линейны $\implies$

$\varphi$ - линейный изоморфизм $\ell_q$ и $\ell_p^*$

Теперь
$\|y\| \leq \|\varphi(y)\| \leq \|\psi \circ \varphi(y)\| = \|y\| \implies \|\varphi(y)\| = \|y\| \implies$

$\varphi$ - изометрия $\implies \boxed{\ell_p^* \cong \ell_q}$

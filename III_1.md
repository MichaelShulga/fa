# Часть III, Задача 1

$A: L_2([0, 1]) \to L_2([0, 1])$

По определению гильбертова сопряженного оператора: $\forall x, y \in (y, Ax) = (A^* y, x)$

**а)** $Ax(t) = \int_0^t t x(s) \, ds = t \int_0^t x(s) \, ds$

$$(y, Ax) = \int_0^1 \overline{y(t)} t \int_0^t x(s) \, ds \, dt = \int_0^1 x(s) \overline{\int_s^1 t \overline{y(t)} \, dt} \, ds = (A^* y, x) \implies$$

$$\boxed{A^* y(s) = \int_s^1 t y(t) \, dt}$$

**б)** $Ax(t) = \int_0^t s x(s) \, ds$

$$(y, Ax) = \int_0^1 \overline{y(t)} \int_0^t s x(s) \, ds \, dt = \int_0^1 x(s) \cdot \overline{\int_s^1 y(t) \, dt} \, ds \implies \boxed{A^* y(s) = s \int_s^1 y(t) \, dt}$$

*(рисунок треугольной области интегрирования)*

Интегралы можно было менять местами, т.к. в обоих случаях интеграл от модуля подынтегральной функции может быть оценен сверху как $\|x\|_2 \cdot \|y\|_2$, т.е. сходится

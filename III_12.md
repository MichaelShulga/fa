# Часть III, Задача 12

$A \in \mathcal{L}(E_1, E_2)$, $\exists A^{-1} \in \mathcal{L}(E_2, E_1)$.

$\forall f \in E_1^* \implies \underset{x \in E_1}{f(x)} = f(A A^{-1} x) = (A^{-1})^* f(Ax) = A^* (A^{-1})^* f(x) \implies$

В силу того, что $f$ и $x$ произвольны, получаем $A^* (A^{-1})^* = \text{Id}_{E_1^*}$

Аналогично $(y = A A^{-1} y)$ получаем, что $(A^{-1})^* A^* = \text{Id}_{E_2^*} \implies (A^*)^{-1} = (A^{-1})^*$ по определению обратного оператора.

$(A^{-1})^* \in \mathcal{L}(E_1^*, E_2^*) \implies (A^*)^{-1} \in \mathcal{L}(E_1^*, E_2^*)$

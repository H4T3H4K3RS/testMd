

Закон распределения: биномиальное распределение

Математическое ожидание: $$M(X)=3 \cdot P_1 \cdot P_2 \cdot P_3 = 3 \cdot 0.04 \cdot 0.02 \cdot 0.01 = 0.00024$$

Мода: $$Mode(X) = 3$$

Дисперсия: $$D(X)=3 \cdot P_1 \cdot P_2 \cdot P_3 \cdot (1 - P_1) \cdot (1 - P_2) \cdot (1 - P_3)=3 \cdot 0.04 \cdot 0.02 \cdot 0.01 \cdot 0.96 \cdot 0.98 \cdot 0.99=0.00022656$$

Функция распределения:

$$P(X=k)=C_3^k \cdot P_1^k \cdot P_2^{3-k} \cdot P_3^{3-k}$$

где $C_n^k$ - коэффициент биномиального распределения.

Вероятность того, что отказавших элементов будет не более n: $$P(X \le n) = P(X=0)+P(X=1)+P(X=2) = C_3^0 \cdot P_1^0 \cdot P_2^3 \cdot P_3^3 + C_3^1 \cdot P_1^1 \cdot P_2^2 \cdot P_3^2 + C_3^2 \cdot P_1^2 \cdot P_2^1 \cdot P_3^1 = 0.9976$$

Ниже приведён код на Python для построения графика функции распределения:

§ Code

import matplotlib.pyplot as plt
import numpy as np

def binomial(n, k, p):
    return np.math.factorial(n) / (np.math.factorial(k) * np.math.factorial(n - k)) * p**k * (1 - p)**(n - k)

p1 = 0.04
p2 = 0.02
p3 = 0.01

x = np.arange(0, 4)
y = np.array([binomial(3, k, p1 * p2 * p3) for k in x])

plt.plot(x, y)
plt.xlabel("Number of non-defective elements")
plt.ylabel("Probability")
plt.show()

§ Output

> 

 
Закон распределения для данной задачи является биномиальным распределением. Математическое ожидание составляет 0.00024, мода равна 3, а дисперсия равна 0.00022656. Также мы можем построить график функции распределения. Вероятность того, что отказавших элементов будет не более n равна 0.9976.
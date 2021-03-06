# Глава 1. Сравнение рисковых ситуаций и простейшие методы расчета страховых тарифов

### §4. Принципы расчета тарифных ставок

Пусть
$D$ - суммарный страховой взнос; <br>
$X$ - суммарный ущерб; <br>
$F(x)$ - распределение риска; <br>
$\lambda$ - некоторый экзогенный параметр. <br>

Тогда $D=\Psi(F(x), \lambda)$

Принципы:
1. Принцип ожидаемого значения.
$D=(1 + \lambda)EX, \lambda \ge 0$.
2. Принцип дисперсии (дисперсионный принцип).
$D=EX + \lambda DX, \lambda \ge 0$.
3. Принцип стандартного отклонения.
$D=EX + \lambda\sqrt{DX}, \lambda \ge 0$.
4. Принцип нулевой полезности.
Пусть $u(y)$ - функция полезности страховщика с обычными свойствами:
$u'(y) > 0, u''(y) \le 0$.
Страховой взнос D определяется как решение уравнения
$Eu(S + D - X) = u(S)$. <br>
4.1 Экспоненциальный принцип.
Для экспоненциальной функции полезности
$u(y) = a^{-1}(1-e^{-ay}), a>0$,
последнее уравнение имеет решение
$D = a^{-1}\ln(Ee^{aX})$.

5. Обобщенный принцип нулевой полезности.
Пусть начальный капитал S - случайная величина.
Страховой взнос D определяется как решение уравнения
$Eu(S+D-X) = Eu(S)$.
Можно показать, что $D$ зависит от совместного распределения случайных величин $X$ и $S$. <br>
5.1 Обобщенный экспоненциальный принцип.
Для экспоненциальной функции полезности
$D=a^{-1} * \ln\frac{Ee^{a(X-S)}}{Ee^{-aS}}$,
и для малых $а$
$D \approx EX + \frac{a}{2}DX = a*cov(X, S)$.

6. Принцип Эсшера.
$D = \frac{EXe^{\lambda X}}{Ee^{\lambda X}}, \lambda > 0$.
Замечание. Принцип Эсшера возникает при минимизации средних потерь страховщика, если функция потерь имеет вид
$L(x, D) = (D - x)^2e^{\lambda x}$.

Пусть $f(x)$ - плотность случайно величины $X$. Имеем 

$$D'(\lambda) = (\frac{\int_0^{+inf}xe^{\lambda x}f(x)dx}{\int_0^{+inf}e^{\lambda x}f(x)dx})' = \frac{(\int_0^{+inf}xe^{\lambda x}f(x)dx)'\int_0^{+inf}e^{\lambda x}f(x)dx}{(\int_0^{+inf}e^{\lambda x}f(x)dx)^2} - \frac{\int_0^{+inf}xe^{\lambda x}f(x)dx (\int_0^{+inf}e^{\lambda x}f(x)dx)'}{(\int_0^{+inf}e^{\lambda x}f(x)dx)^2} = $$


$$ = \frac{\int_0^{+inf}x^2e^{\lambda x}f(x)dx\int_0^{+inf}e^{\lambda x}f(x)dx}{(\int_0^{+inf}e^{\lambda x}f(x)dx)^2} - \frac{(\int_0^{+inf}xe^{\lambda x}f(x)dx)^2}{(\int_0^{+inf}e^{\lambda x}f(x)dx)^2} = EZ^2 - (EZ)^2 = DZ > 0$$

где $z$ имеет плотность $\frac{e^{\lambda x}f(x)dx}{\int_0^{+inf}e^{\lambda x}f(x)dx}, x>0$.

Таким образом, $D(\lambda)$ - возрастающая функиця от $\lambda$; параметр $\lambda$ характеризует неприятие риска страховой компанией при $\lambda = 0$ действует приницп эквивалентности ($D = EX$).

7. Швейцарсикй принцип.
Страховой взнос $D$ определяется как решение уравнения 
$Eg(X-\lambda D) = g((1-\lambda)D), \lambda \in [0, 1]$,
где $g(x)$ - вещественная непрерывная функция, обладающая свойствами $g'(x) > 0, g''(x) \ge 0$ <br>
При $\lambda = 0$ действует обобщенный принцип эквивалентности 
$D = g^{-1}(Eg(x))$ <br>
При $\lambda = 1$:

- действует принцип нулевой полезности относительно функции полезности
$u(y) = -g(S-y)$
- действует экспоненциальный принцип 
$g(x) = a^{-1}(e^{ax} - 1), a > 0$
- действует принцип Эсшера
$g(x) = xe^{ax}, a > 0$

8. Принцип Орлича.
Страховой взнос $D$ определяется как решение уравнения $E\rho(XD^{-\lambda}) = \rho(D^(1-\lambda))$, 
где $\lambda X \in [0, 1]$ и $\rho(x)$ - непрерывная строго возрастающая функция. 
При $\lambda = 0$ получается обобщенный принцип эквивалентности.
9. Квантильный принцип.
Пусть $F^{<-} (y) = \inf\{x \in R|F(x) \ge y\}, 0 < y < 1$,
левая $y$-квантиль раcпределения риска.
Пусть величина $Q<1$ близка к единиц. В этом случае $D = F^*(Q)$.
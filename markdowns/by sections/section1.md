# Глава 1. Сравнение рисковых ситуаций и простейшие методы расчета страховых тарифов

### §1. Понятие об общей теории оценивания риска

Пусть
$n$ - число страховых полисов в портфеле; <br>
$S$ - начальный капитал страховщика; <br>
$X_i$ - $i$-й индивидуальный иск с функцией распределения $F_i(x)$; <br>
$X = X_1 + … + X_n$ - общие страховые выплаты;

**Определение**. Функция распределения общих страховых выплат $X$: <br>
$F(x) = P(X < x), x \in R$
называется распределением риска страховой компании.

Пусть $\mu = EX < \inf$ <br>
**Определение**. Число $\mu_n = \frac{\mu}{n}$ называется чистой ценой (рисковой премией). Если страховая и рисковая премии равны, то говорят о действии приницпа эквивалентности.

Пусть $v_i$ - нагрузка (рисковая надбавка), соответствующая $i$-му полису. Тогда прирост капитала страховщика имеет вид:
$S + \sum_{i=1}^nv_i + \mu = R + \mu$

**Определение**. Величина $R$ называется свободным резервом. <br>
Пара $(R, F(x))$ называется рисковой ситуацией. <br>
Пусть $Y = R + \mu - Х$ - конечный капитал страховой компании. Обозначим через $G(y)$ функцию распределения $Y$. <br>
Имеем 

$$G(y) = P(Y < y) = P(R + \mu - X < y) = 1 - F(R + \mu - y + 0)$$
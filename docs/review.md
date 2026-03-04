# 幂级数与泰勒级数：理论速查

## 一、 幂级数与收敛域

**标准形式**：$\sum_{n=0}^{\infty} a_n (x-a)^n$



**1. 收敛半径 $R$ 的计算**
提取系数 $a_n$，计算以下极限（通常使用比值法）：
* **比值法**：$R = \lim_{n \to \infty} \left| \frac{a_n}{a_{n+1}} \right|$
* **根值法**：$R = \lim_{n \to \infty} \frac{1}{\sqrt[n]{|a_n|}}$

**2. 收敛区间判定法则**
* 区间内部 $(a-R, a+R)$：绝对收敛。
* 区间外部 $|x-a| > R$：发散。
* **端点 $x = a \pm R$：必须代入原级数，使用常数项级数判别法单独检验。**

---

## 二、 泰勒级数与麦克劳林级数



**1. 泰勒级数 (在 $x=a$ 处展开)**：
$$f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n$$

**2. 麦克劳林级数 (在 $x=0$ 处展开)**：
$$f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(0)}{n!} x^n$$

---

## 三、 常用麦克劳林展开式

| 函数 $f(x)$ | 展开式 | 收敛区间 |
| :--- | :--- | :--- |
| **$e^x$** | $\sum_{n=0}^{\infty} \frac{x^n}{n!} = 1 + x + \frac{x^2}{2!} + \dots$ | $(-\infty, \infty)$ |
| **$\sin x$** | $\sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{(2n+1)!} = x - \frac{x^3}{3!} + \dots$ | $(-\infty, \infty)$ |
| **$\cos x$** | $\sum_{n=0}^{\infty} \frac{(-1)^n x^{2n}}{(2n)!} = 1 - \frac{x^2}{2!} + \dots$ | $(-\infty, \infty)$ |
| **$\frac{1}{1-x}$** | $\sum_{n=0}^{\infty} x^n = 1 + x + x^2 + \dots$ | $(-1, 1)$ |
| **$\ln(1+x)$** | $\sum_{n=1}^{\infty} \frac{(-1)^{n-1} x^n}{n} = x - \frac{x^2}{2} + \dots$ | $(-1, 1]$ |
| **$(1+x)^k$** | $\sum_{n=0}^{\infty} \binom{k}{n} x^n = 1 + kx + \dots$ | 视 $k$ 而定 |
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

# Κεφάλαιο 4 - Ολοκληρώματα

[επιστροφή στα περιεχόμενα](./README.md)



## Άσκηση 4.1


**Περιγραφή**

Από τις αρχικές συναρτήσεις (παράγουσες) της $f(x)=x^{1/3}$ να προσδιοριστεί εκείνη της οποίας η γραφική παράσταση
περνά από το σημείο (1,2).

**Λύση**

$$
\begin{aligned}
& f(x)=x^{1 / 3} \\
& \left.\begin{array}{c}
F(x)=\frac{x^{4 / 3}}{\frac{4}{3}}+c=\frac{3}{4} x^{4 / 3}+c \\
F(1)=2
\end{array}\right\} \Rightarrow \frac{3}{4} 1^{4 / 3}+c=2 \Rightarrow c=\frac{5}{4} \\
& F(x)=\frac{3}{4} x^{4 / 3}+\frac{5}{4} \\
&
\end{aligned}
$$

---

## Άσκηση 4.2


**Περιγραφή**

Να προσδιοριστεί η $f(x)$ για την οποία ισχύει $f''(x)=6x+2$, $f(1)=5$, $f(2)=7$.

**Λύση**

$$f^{\prime}(x)=6 \frac{x^2}{2}+2 x+c_1=3 x^2+2 x+c_1 $$

$$f(x)=3 \frac{x^3}{3}+2 \frac{x^2}{2}+c_1 x+c_2=x^3+x^2+c_1 x+c_2 .$$

$$
\left.\begin{array}{l}
f(1)=5 \Rightarrow c_1+c_2=5-2 \Rightarrow c_1+c_2=3 \\
f(2)=7 \cdot 2^3+2^2+2 c_1+c_2=7 \Rightarrow 2 c_1+c_2=-5
\end{array}\right\} \Rightarrow \begin{aligned}
& c_1=-8 \\
& c_2=11
\end{aligned}
$$


---

## Άσκηση 4.3


**Περιγραφή**

Να υπολογιστούν τα ολοκληρώματα 

$$ \alpha) \; \int \frac{3 x^2-2 x+5}{x} d x$$ 

$$\beta) \; \int \frac{\sqrt{x}+1}{x} d x$$

**Λύση**


α)

$$ \int \frac{3 x^2-2 x+5}{x} d x=\int\left(3 x-2+5 \frac{1}{x}\right) d x=3 \frac{x^2}{2}-2 x+5 \ln |x|+c $$

β)

$$ \int \frac{\sqrt{x}+1}{x} d x=\int\left(\frac{1}{\sqrt{x}}+\frac{1}{x}\right) d x=\frac{x^{1 / 2}}{\frac{1}{2}}+\ln x+c=2 \sqrt{x}+\ln |x|+c $$



---

## Άσκηση 4.4


**Περιγραφή**

Να προσδιοριστούν οι τιμές του $b$ ώστε να ισχύει 

$$\int_b^{2 b}-2 x d x=-48$$

**Λύση**

$$
\begin{aligned}
& \int_b^{2 b}-2 x d x=-48 \Rightarrow \\
& -2 \int_b^{2 b} x d x=-48 \Rightarrow\\
& -2\left[\frac{x^2}{2}\right]_b^{2 b}=-48 \Rightarrow \\
& -4 b^2+b^2=-48 \Rightarrow\\
& b^2=16 \Rightarrow \\
& b= \pm 4
\end{aligned}
$$


---

## Άσκηση 4.5


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$\int_{-1}^0 x(x-2)(x+2) d x$$

**Λύση**

$$
\begin{aligned}
& \int_{-1}^0 x(x-2)(x+2) d x=\int_{-1}^0 x\left(x^2-4\right) d x=\int_{-1}^0\left(x^3-4 x\right) d x= \\
& =\left[\frac{x^4}{4}\right]_{-1}^0-4\left[\frac{x^2}{2}\right]_{-1}^0=-\frac{(-1)^4}{4}-4\left(-\frac{(-1)^2}{2}\right)=-\frac{1}{4}+2=\frac{7}{4}
\end{aligned}
$$


---

## Άσκηση 4.6


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$\int_{-1}^2(|x|+2|x-1|) d x$$

**Λύση**

$$
\begin{aligned}
& \int_{-1}^2(|x|+2|x-1|) d x= \\
= & \int_{-1}^0(|x|+2|x-1|) d x+\int_0^1(|x|+2|x-1|) d x+\int_1^2(|x|+2|x-1|) d x= \\
= & \int_{-1}^0(-x-2(x-1)) d x+\int_0^1(x-2(x-1)) d x+\int_1^2(x+2(x-1)) d x= \\
= & \int_{-1}^0(-3 x+2) d x+\int_0^1(-x+2) d x+\int_1^2(3 x-2) d x= \\
= & -3\left[\frac{x^2}{2}\right]_{-1}^0+2[x]_{-1}^0-\left[\frac{x^2}{2}\right]_0^1+2[x]_0^1+3\left[\frac{x^2}{2}\right]_1^2-2[x]_1^2= \\
= & -\frac{3}{2}(0-1)+2(0+1)-\frac{1}{2}(1-0)+2(1-0)+\frac{3}{2}(4-1)-2(2-1)= \\
= & \frac{3}{2}+2-\frac{1}{2}+2+\frac{9}{2}-2= \\
= \frac{11}{2}+2= \\
= \frac{15}{2}
\end{aligned}
$$


---

## Άσκηση 4.7


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$\int_1^e x \ln x d x$$

**Λύση**

$$
\begin{aligned}
& \int_1^e x \ln x d x= \\
& =\int_1^e \frac{1}{2}\left(x^2\right)' \ln x d x= \\
& =\frac{1}{2}\left[x^2 \ln x\right]_1^e-\frac{1}{2} \int_1^e x^2(\ln x)' d x= \\
& =\frac{1}{2}\left[e^2 \ln e-1 \ln 1\right]-\frac{1}{2} \int_1^e x^2 \frac{1}{x} d x= \\
& =\frac{1}{2} e^2-\frac{1}{2} \int_1^e x d x= \\
& =\frac{1}{2} e^2-\frac{1}{2}\left[\frac{x^2}{2}\right]_1^e= \\
& =\frac{e^2}{2}-\frac{1}{2}\left(\frac{e^2-1}{2}\right)= \\
& =\frac{1}{4}\left(e^2+1\right)
\end{aligned}
$$


---

## Άσκηση 4.8


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$\int_1^e x^2 \ln x d x$$

**Λύση**

$$
\begin{aligned}
& \int_1^e x^2 \ln x d x= \\
& =\int_1^e\left(\frac{x^3}{3}\right)' \ln x d x =\\
& =\left[\frac{x^3}{3} \ln x\right]_1^e-\int_1^e \frac{x^3}{3}(\ln x)' d x= \\
& = \frac{e^3}{3} \ln e-\frac{1}{3} \ln 1-\int_1^e \frac{x^3}{3} \frac{1}{x} d x=\\
& =\frac{1}{3} e^3-\frac{1}{3} \int_1^e x^2 d x= \\
& =\frac{1}{3} e^3-\frac{1}{3}\left[\frac{x^3}{3}\right]_1^e=\\
& =\frac{1}{3} e^3-\frac{1}{9} e^3+\frac{1}{9}=\\
& =\frac{2 e^3+1}{9}
\end{aligned}
$$

---

## Άσκηση 4.9


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$\int \frac{x}{1+x^2} d x$$

**Λύση**

$$
\begin{aligned}
& \int \frac{x}{1+x^2} d x=\frac{1}{2} \int \frac{\left(1+x^2\right)^{\prime}}{1+x^2} d x \\
& \\
& u(x)=1+x^2 \Rightarrow u'(x) dx=d u \Rightarrow\left(1+x^2\right)' dx=du \Rightarrow 2x dx=du\\
& \\
& \int \frac{x}{1+x^2} d x=\frac{1}{2} \int \frac{1}{u} d u=\frac{1}{2} \ln |u|+c=\frac{1}{2} \ln \left(1+x^2\right)+c
\end{aligned}
$$

---

## Άσκηση 4.10


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$ \int x e^{x^2+1} d x$$

**Λύση**

$$
\begin{aligned}
& \int x e^{x^2+1} d x=\frac{1}{2} \int\left(x^2+1\right)' e^{x^2+1} d x \\
& \\
& x^2+1=u \Rightarrow\left(x^2+1\right)^{\prime} d x=d u \Rightarrow 2 x d x=d u \\
& \\
& \int  x e^{x^2+1} d x=\frac{1}{2} \int\left(x^2+1\right)^{\prime} e^{x^2+1} d x=\frac{1}{2} \int e^u d u=\frac{1}{2} e^u+c=\frac{1}{2} e^{x^2+1}+c
\end{aligned}
$$

---

## Άσκηση 4.11


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$\int_0^1 x^2 e^{x^3+1} d x$$

**Λύση**

$$
\begin{aligned}
& \int_0^1 x^2  e^{x^3+1} d x=\frac{1}{3} \int_0^1\left(x^3+1\right)' e^{x^3+1} d x \\
& x^3+1=u \rightarrow 3 x^2 d x=d u \\
& x=0 \Rightarrow u=1 \\
& x=1 \Rightarrow u=2 \\
& \int_0^1 x^2 e^{x^3+1} d x=\frac{1}{3} \int_1^2 e^u d u=\frac{1}{3}\left[e^u\right]_1^2=\frac{1}{3}\left(e^2-e\right)
\end{aligned}
$$

---

## Άσκηση 4.12


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα 

$$\int_0^3 \sqrt{1+x} d x$$

**Λύση**

$$
\begin{aligned}
& \int_0^3 \sqrt{1+x} d x \\
& u(x)=1+x \Rightarrow du=dx  \\
& x=0 \Rightarrow u=1 \\
& x=3 \Rightarrow u=4
\end{aligned}
$$

Συνεπώς

$$
\begin{aligned}
& \int_0^3 \sqrt{1+x} d x=\int_1^4 \sqrt{u} d u= \\
& = \left[\frac{u^{3 / 2}}{\frac{3}{2}}\right]_1^4= \left( \sqrt{4^3}- \sqrt{1^3} \right) =\\
&=\frac{2}{3}(8-1)=\frac{14}{3}
\end{aligned}
$$

---

## Άσκηση 4.13


**Περιγραφή**

Να υπολογιστεί το ολοκλήρωμα $$\int_0^2 x \sqrt{4-x^2} d x$$

**Λύση**

$$
\begin{aligned}
& \int_0^2 x \sqrt{4-x^2} d x=-\frac{1}{2} \int_0^2\left(4-x^2\right)' \sqrt{4-x^2} d x \\
& u(x)=4-x^2 \Rightarrow d u=-2 x d x \\
& u(0)=4-0^2=4 \\
& u(2)=4-2^2=0
\end{aligned}
$$

Συνεπώς

$$\int_0^2 x \sqrt{4-x^2} d x=-\frac{1}{2} \int_4^0 \sqrt{u} d u=\frac{1}{2} \int_0^4 \sqrt{u} d u=\frac{1}{2}\left[\frac{u^{3 / 2}}{\frac{3}{2}}\right]_0^4=\frac{1}{2} \frac{2}{3} \sqrt{4^3}=\frac{8}{3}$$

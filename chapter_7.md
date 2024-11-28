<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

# Κεφάλαιο 7 - Πίνακες - Ορίζουσες

[επιστροφή στα περιεχόμενα](./README.md)



## Άσκηση 7.1

**Περιγραφή**

Να υπολογιστεί η ορίζουσα: 

$$
\left|\begin{array}{cccc}
4 & 0 & -3 & 5 \\
0 & 6 & 0 & 0 \\
1 & 3 & -4 & 2 \\
3 & -1 & 2 & 0
\end{array}\right|
$$

**Λύση**

$$
\left|
\begin{array}{cccc}
4 & 0 & -3 & 5 \\
0 & 6 & 0 & 0 \\
1 & 3 & -4 & 2 \\
3 & -1 & 2 & 0
\end{array}
\right|
=6\left|
\begin{array}{ccc}
4 & -3 & 5 \\
1 & -4 & 2 \\
3 & 2 & 0
\end{array}
\right|=
$$

$$
= 6\left(\begin{array}{cc}
3 & \left.\left|
\begin{array}{cc}
-3 & 5 \\
-4 & 2
\end{array}
\right|
-2\left|
\begin{array}{ll}
4 & 5 \\
1 & 2
\end{array}
\right|
\right)=
\end{array}\right.
$$

$$
= 6 \left( 3(-6+20)-2(8-5) \right)=6(42-6)=216
$$


---

## Άσκηση 7.2

**Περιγραφή**


Να δείξετε ότι ισχύει:

$$
\left|\begin{array}{llll}
\alpha & \beta & 0 & 0 \\
\gamma & \delta & 0 & 0 \\
0 & 0 & \kappa & \lambda \\
0 & 0 & \mu & \nu
\end{array}\right|=
\left|\begin{array}{ll}
\alpha & b \\
\gamma & \delta
\end{array}\right|
\left|\begin{array}{ll}
\kappa & \lambda \\
\mu & \nu
\end{array}\right|
$$

**Λύση**


$$
\left|\begin{array}{llll}
\alpha & \beta & 0 & 0 \\ 
\gamma & \delta & 0 & 0 \\
0 & 0 & \kappa & \lambda \\
0 & 0 & \mu & \nu
\end{array}\right|=
\alpha
\left|\begin{array}{lll}
\delta & 0 & 0 \\
0 & \kappa & \lambda \\
0 & \mu & \nu
\end{array}\right|
-\beta
\left|\begin{array}{lll}
\gamma & 0 & 0 \\
0 & \kappa & \lambda \\
0 & \mu & \nu
\end{array}\right|= 
$$

$$
=\alpha \left(\delta \cdot\left|
\begin{array}{cc}
\kappa & \lambda \\
\mu & \nu
\end{array}
\right|\right)
-\beta\left(\gamma \left|
\begin{array}{ll}
\kappa & \lambda \\
\mu & \nu
\end{array}\right|\right)= 
$$

$$
=(\alpha \delta-\beta \gamma)\left|
\begin{array}{ll}
\kappa & \lambda \\
\mu & \nu
\end{array}
\right|=
\left|\begin{array}{ll}
\alpha & \beta \\
\gamma & \delta
\end{array}\right|
\left|\begin{array}{ll}
\kappa & \lambda \\
\mu & \nu
\end{array}\right|
$$

---


## Άσκηση 7.3

**Περιγραφή**

Να υπολογιστεί η ορίζουσα

$$
\left|\begin{array}{llllll}
0 & 0 & 0 & 0 & 0 & 1 \\ 
0 & 0 & 0 & 0 & 2 & 1 \\ 
0 & 0 & 0 & 3 & 2 & 1 \\ 
0 & 0 & 4 & 3 & 2 & 1 \\ 
0 & 5 & 4 & 3 & 2 & 1 \\ 
6 & 5 & 4 & 3 & 2 & 1
\end{array}\right|
$$

**Λύση**


$$
\underset{\Gamma_{1} \leftrightarrow \Gamma_{6}}{=}-\left|
\begin{array}{llllll}
6 & 5 & 4 & 3 & 2 & 1 \\
0 & 0 & 0 & 0 & 2 & 1 \\
0 & 0 & 0 & 3 & 2 & 1 \\
0 & 0 & 4 & 3 & 2 & 1 \\
0 & 5 & 4 & 3 & 2 & 1 \\
0 & 0 & 0 & 0 & 0 & 1
\end{array}\right| 
$$

$$
\underset{\Gamma_{2} \leftrightarrow \Gamma_{5}}{=}\left|
\begin{array}{llllll}
6 & 5 & 4 & 3 & 2 & 1 \\
0 & 5 & 4 & 3 & 2 & 1 \\
0 & 0 & 0 & 3 & 2 & 1 \\
0 & 0 & 4 & 3 & 2 & 1 \\
0 & 0 & 0 & 0 & 2 & 1 \\
0 & 0 & 0 & 0 & 0 & 1
\end{array}\right|=
$$

$$
\underset{\Gamma_{3} \leftrightarrow \Gamma_{4}}{=}-\left|
\begin{array}{llllll}
6 & 5 & 4 & 3 & 2 & 1 \\
0 & 5 & 4 & 3 & 2 & 1 \\
0 & 0 & 4 & 3 & 2 & 1 \\
0 & 0 & 0 & 3 & 2 & 1 \\
0 & 0 & 0 & 0 & 2 & 1 \\
0 & 0 & 0 & 0 & 0 & 1
\end{array}\right|=
$$

$$
=-6 \cdot 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1=-720
$$

---

## Άσκηση 7.4

**Περιγραφή**

Να βρείτε το $x$ αν ισχύει:

$$
\left|\begin{array}{ccc}
1 & -1 & 3 \\
2 & x & 2 \\
3 & 0 & 4
\end{array}\right|=0
$$

**Λύση**

$$
\left|\begin{array}{ccc}
1 & -1 & 3 \\
2 & x & 2 \\
3 & 0 & 4
\end{array}\right|=0 \quad 
\underset{\Gamma_{2} : \Gamma_{2}-2\Gamma_{1}}{\Longrightarrow}
\left|
\begin{array}{ccc}
1 & -1 & 3 \\
0 & x+2 & -4 \\
3 & 0 & 4
\end{array}
\right|=0 
\underset{\Gamma_{3} : \Gamma_{3}-3\Gamma_{1}}{\Longrightarrow}
$$

$$
\Rightarrow\left|\begin{array}{ccc}
1 & -1 & 3 \\
0 & x+2 & -4 \\
0 & 3 & -5
\end{array}\right|=0 \Rightarrow\left|\begin{array}{cc}
x+2 & -4 \\
3 & -5
\end{array}\right|=0 
$$

$$
\Rightarrow-5 x-10+12=0
\Rightarrow x=2/5
$$

---


## Άσκηση 7.5

**Περιγραφή**

Να υπολογιστεί η ορίζουσα

$$
\left|\begin{array}{cccc}
1 & 1 & 1 & 1 \\
1 & -1 & 1 & 1 \\
1 & 1 & -1 & 1 \\
1 & 1 & 1 & -1
\end{array}\right|
$$

**Λύση**


$$
\left|\begin{array}{cccc}
1 & 1 & 1 & 1 \\
1 & -1 & 1 & 1 \\
1 & 1 & -1 & 1 \\
1 & 1 & 1 & -1
\end{array}\right| 
\quad
\begin{aligned}
&\Gamma_{2} : \Gamma_{2}-\Gamma_{1} \\
&\Gamma_{3} : \Gamma_{3}-\Gamma_{1} \\
&\Gamma_{4} : \Gamma_{4}-\Gamma_{1} \\
& \Longrightarrow
\end{aligned}
$$

$$
\Rightarrow
\left|\begin{array}{cccc}
1 & 1 & 1 & 1 \\
0 & -2 & 0 & 0 \\
0 & 0 & -2 & 0 \\
0 & 0 & 0 & -2
\end{array}\right|=
$$

$$
=1 (-2)(-2)(-2)=-8
$$

---

## Άσκηση 7.6

**Περιγραφή**

Να υπολογιστεί η ορίζουσα του πίνακα Α

$$
A=\left[\begin{array}{ccc}
-a & a-1 & a+1\\
1 & 2 & 3\\
2-a & a+3 & a+7\\
\end{array}\right]
$$

**Λύση**

$$
\left|\begin{array}{ccc}
-a & a-1 & a+1\\
1 & 2 & 3\\
2-a & a+3 & a+7\\
\end{array}\right|
\overset{\Gamma_3:\Gamma_3-2\Gamma_2}{=}
$$

$$
\left|\begin{array}{ccc}
-a & a-1 & a+1\\
1 & 2 & 3\\
-a & a-1 & a+1\\
\end{array}\right|=0
$$

---

## Άσκηση 7.7

**Περιγραφή**

Να δείξετε ότι ισχύει

$$
\left|
\begin{array}{ccc}
1-\alpha-b & c & c \\
\alpha & 1-b-c & \alpha \\
b & b & 1-c-\alpha
\end{array}
\right|
\geq 0
$$

**Λύση**

$$
\left|
\begin{array}{cccc|ccc|c}
1-\alpha-b & c & c \\
\alpha & 1-b-c & \alpha \\
b & b & 1-c-\alpha
\end{array}
\right|
\overset{\Gamma_1:\Gamma_1+\Gamma_2+\Gamma_3}{=}
$$

$$
\left|
\begin{array}{cccc|ccc|c}
1 & 1 & 1 \\
\alpha & 1-b-c & \alpha \\
b & b & 1-c-\alpha
\end{array}
\right|
\overset{\Sigma_2:\Sigma_2-\Sigma_1}{=}
$$

$$
\left|
\begin{array}{cccc|ccc|c}
1 & 0 & 1 \\
\alpha & 1-\alpha-b-c & \alpha \\
b & 0 & 1-c-\alpha
\end{array}
\right|
\overset{\Sigma_3:\Sigma_3-\Sigma_1}{=}
$$

$$
\left|\begin{array}{ccc}
1 & 0 & 0 \\
\alpha & 1-\alpha-b-c & 0 \\
b & 0 & 1-b-c-\alpha
\end{array}\right|=
$$

$$
=(1-\alpha-b-c)^{2} \geq 0
$$



[επιστροφή στα περιεχόμενα](./README.md)
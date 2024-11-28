<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

# Κεφάλαιο 6 - Πίνακες

[επιστροφή στα περιεχόμενα](./README.md)



## Άσκηση 6.1

**Περιγραφή**

Δίνεται ο πίνακας Α. Να βρεθεί ο λ ώστε να ισχύει $ A=A^T $

$$
A=\left[\begin{array}{ccc}
1 & \lambda & 0 \\
2-\lambda & 2 & 1 \\
0 & \lambda^{2} & 3
\end{array}\right]
$$


**Λύση**

$$
A^{T}=\left[\begin{array}{ccc}1 & 2-\lambda & 0 \\\lambda & 2 & \lambda^{2} \\0 & 1 & 3\end{array}\right]
$$

$$
A=A^{T} \Leftrightarrow\left[\begin{array}{ccc}1 & \lambda & 0 \\2-\lambda & 2 & 1 \\0 & \lambda^{2} & 3\end{array}\right]=\left[\begin{array}{ccc}1 & 2-\lambda & 0 \\\lambda & 2 & \lambda^{2} \\0 & 1 & 3\end{array}\right]
$$

$$
\left.\left.\begin{array}{l}\lambda=2-\lambda \\\lambda^{2}=1 .\end{array}\right\} \Rightarrow \begin{array}{l}2 \lambda=2 \\(\lambda-1)(\lambda+1)=0\end{array}\right\}
\Rightarrow
\lambda=1
$$


---

## Άσκηση 6.2

**Περιγραφή**

Να βρεθούν οι πίνακες Χ και Υ αν ισχύει:

$$
\begin{aligned}
& \begin{array}{l}2 X+3 \Psi=\left[\begin{array}{ll}3 & 0 \\0 & 3\end{array}\right] \\3 X-2 \Psi=\left[\begin{array}{cc}-2 & 0 \\0 & -2\end{array}\right]\end{array}
\end{aligned}
$$

**Λύση**

$$
\begin{aligned}
& \left.\begin{array}{l}2 X+3 \Psi=\left[\begin{array}{ll}3 & 0 \\0 & 3\end{array}\right] \\3 X-2 \Psi=\left[\begin{array}{cc}-2 & 0 \\0 & -2\end{array}\right]\end{array}\right\} \Leftrightarrow \\
& \left.\begin{array}{l}4 X+6 \Psi=\left[\begin{array}{ll}6 & 0 \\0 & 6\end{array}\right] \\9 X-6 \Psi=\left[\begin{array}{cc}-6 & 0 \\0 & -6\end{array}\right]\end{array}\right\} \Leftrightarrow \\
& \left.\begin{array}{l}13 X=\left[\begin{array}{ll}0 & 0 \\0 & 0\end{array}\right] \\3 X-2 \Psi=\left[\begin{array}{cc}-2 & 0 \\0 & -2\end{array}\right]\end{array}\right\} \Leftrightarrow \\
& X=\left[\begin{array}{cc}0 & 0 \\0 & 0\end{array}\right]  \\
& \Psi=\frac{1}{(-2)}\left[\begin{array}{cc}-2 & 0 \\0 & -2\end{array}\right] \Leftrightarrow \Psi=\left[\begin{array}{ll}1 & 0 \\0 & 1\end{array}\right]
\end{aligned}
$$



---

## Άσκηση 6.3

**Περιγραφή**

Να βρεθεί ο $f(A)$ αν $f(x)=x^2 - 1$ και 

$$
A=\left[\begin{array}{cc}
0 & 1 \\
1 & -2
\end{array} \right]
$$

**Λύση**

$$
\begin{aligned}
f(A)=A^{2}-I &=\left[\begin{array}{cc}
0 & 1 \\
1 & -2
\end{array}\right] \cdot\left[\begin{array}{cc}
0 & 1 \\
1 & -2
\end{array}\right]-\left[\begin{array}{ll}
1 & 0 \\
0 & 1
\end{array}\right]=\\
&=\left[\begin{array}{cc}
1 & -2 \\
-2 & 5
\end{array}\right]-\left[\begin{array}{cc}
1 & 0 \\
0 & 1
\end{array}\right]=\left[\begin{array}{cc}
0 & -2 \\
-2 & 4
\end{array}\right]
\end{aligned}
$$




---

## Άσκηση 6.4

**Περιγραφή**

Δίνεται ο πίνακας Α

$$
A=\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 2 & -1 \\
1 & -1 & 0
\end{array}\right]
$$
Να δείξετε ότι $A^3-3A^2+3I_3=0$ και να βρεθεί ο $A^{-1}$


**Λύση**


$$
\begin{aligned}
&A^{2}=\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 2 & -1 \\
1 & -1 & 0
\end{array}\right]\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 2 & -1 \\
1 & -1 & 0
\end{array}\right]=\left[\begin{array}{ccc}
2 & -1 & 1 \\
-1 & 5 & -2 \\
1 & -2 & 2
\end{array}\right] \\
&A^{3}=\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 2 & -1 \\
1 & -1 & 0
\end{array}\right]\left[\begin{array}{ccc}
2 & -1 & 1 \\
-1 & 5 & -2 \\
1 & -2 & 2
\end{array}\right]=\left[\begin{array}{ccc}
3 & -3 & 3 \\
-3 & 12 & -6 \\
3 & -6 & 3
\end{array}\right]
\end{aligned}
$$

$$
\begin{aligned}
A^{3}-3 A^{2}+3 I_{3} &=\left[\begin{array}{ccc}
3 & -3 & 3 \\
-3 & 12 & -6 \\
3 & -6 & 3
\end{array}\right]-3\left[\begin{array}{ccc}
2 & -1 & 1 \\
-1 & 5 & -2 \\
1 & -2 & 2
\end{array}\right]+3\left[\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right] \\
&=\left[\begin{array}{ccc}
3-6+3 & -3+3+0 & 3-3+0 \\
-3+3+0 & 12-15+3 & -6+6+0 \\
3-3+0 & -6+6+0 & 3-6+3
\end{array}\right]=0
\end{aligned}
$$

$A^{3}-3 A^{2}+3 I_{3}=0 \Leftrightarrow A^{3}-3 A^{2}=-3 I_{3} \Leftrightarrow$

$\Leftrightarrow\left(A^{2}-3 A\right) \cdot A=-3 I_{3} \Leftrightarrow\left[-\frac{1}{3}\left(A^{2}-3 A\right)\right] A=I_{3}$

Επομένως

$$
 A^{-1}=-\frac{1}{3}\left(A^{2}-3 A\right)
$$


---

## Άσκηση 6.5

**Περιγραφή**

Δίνεται $(A+2I_n)^2 = 0$. Να δείξετε ότι οι πίνακες $A$ και $(A+I_n)$ είναι αντιστρέψιμοι.

**Λύση**

$$
\begin{aligned}
&\left(A+2 I_{n}\right)^{2}=0 \Leftrightarrow A^{2}+A\left(2 I_{n}\right)+2\left(I_{n} A\right)+4 I_{n}^{2}=0 \\
&A^{2}+2 A+2 A+4 I_{n}=0 \Leftrightarrow A^{2}+4 A+4 I_{n}=0 \\
&\Leftrightarrow A^{2}+4 A=-4 I_{n} \Leftrightarrow-\frac{1}{4} A^{2}-A=I_{n}(1)
\end{aligned}
$$


$$
(1) \Rightarrow \left(-\frac{1}{4} A-I_{n}\right) A=I_{n}
$$

$$
(1) \Rightarrow A\left(-\frac{1}{4} A-I_{n}\right)=I_{n}
$$

Επομένως $A^{-1}=-\frac{1}{4} A-I_{n}$

$\begin{aligned}
& \left(A+2 I_{n}\right)^{2}=0 \Leftrightarrow A^{2}+4 A+4 I_{n}=0 \Leftrightarrow \\
& 4\left(A+I_{n}\right)=-A^{2} \Leftrightarrow A+I_{n}=\left(-\frac{1}{4}\right) A^{2}  \quad (2)\\
\end{aligned}$

$$
\begin{aligned}
& (2) \Rightarrow\left[-4\left(A^{-1}\right)^{2}\right]\left(A+I_{n}\right)=\left[-4\left(A^{-1}\right)^{2}\right]\left(-\frac{1}{4}\right) A^{2} \\
& \Leftrightarrow-4 \cdot\left(A^{-1}\right)^{2}\left(A+I_{n}\right)=A^{-1} \cdot A^{-1} A \quad A \\
& \Leftrightarrow-4\left(A^{-1}\right)^{2}\left(A+I_{n}\right)=I_{n} \\
\end{aligned}
$$

$$
\begin{aligned}
& (2) {\Rightarrow}\left(A+I_{n}\right)\left[-4\left(A^{-1}\right)^{2}\right]=\left(-\frac{1}{4} A^{2}\right)\left[-4\left(A^{-1}\right)^{2}\right] \\
& \Leftrightarrow(A+I n)\left[-4\left(A^{-1}\right)^{2}\right]=I_n \\
& \left(A+I_{n}\right)^{-1}=-4 \cdot\left(A^{-1}\right)^{2}=-4 A^{-2}
\end{aligned}
$$


---

## Άσκηση 6.6

**Περιγραφή**

Δίνεται ο πίνακας.

$$
A=\left[\begin{array}{cc}
\lambda & 1+\lambda \\
1-\lambda & -\lambda
\end{array}\right]
$$

α) Να δείξετε ότι $A^2=I_2$ και ότι $A^{-1}=A$

β) Για $\lambda=2$ να βρεθεί ο πίνακας Β για τον οποίο ισχύει $A^{99}B=\left[\begin{array}{cc}
1 & 1 \\
2 & 3
\end{array}\right]$

**Λύση α)**

$$
\begin{aligned}
&A^{2}=\left[\begin{array}{cc}
\lambda & 1+\lambda \\
1-\lambda & -\lambda
\end{array}\right]\left[\begin{array}{cc}
\lambda & 1+\lambda \\
1-\lambda & -\lambda
\end{array}\right]=\left[\begin{array}{cc}
\lambda^{2}+(1-\lambda)(1+\lambda) & \lambda(1+\lambda)-\lambda(1+\lambda) \\
\lambda(1-\lambda)-\lambda(1-\lambda) & (1-\lambda)(1+\lambda)+\lambda^{2}
\end{array}\right] \\
&A^{2}=\left[\begin{array}{cc}
\lambda^{2}+1-\lambda^{2} & 0 \\
0 & 1-\lambda^{2}+\lambda^{2}
\end{array}\right]=\left[\begin{array}{ll}
1 & 0 \\
0 & 1
\end{array}\right] \\
&A \cdot A=I \Rightarrow A^{-1}=A .
\end{aligned}
$$

**Λύση β)**

$$
\begin{aligned}
& A^{99}=A^{98} \cdot A=\left(A^{2}\right)^{49} \cdot A=I^{49} \cdot A=A \text {. } \\
& \left.\begin{array}{l}A^{99} \cdot B=A \cdot B= \\A^{99} \cdot B=\left[\begin{array}{ll}1 & 1 \\2 & 3\end{array}\right]\end{array}\right\} \Rightarrow A \cdot B=\left[\begin{array}{cc}1 & 1 \\2 & 3\end{array}\right] \Leftrightarrow A^{-1} \cdot(A \cdot B)=A^{-1} \cdot\left[\begin{array}{cc}1 &1\\2 & 3\end{array}\right] \\
& \Leftrightarrow B=A^{-1}\left[\begin{array}{ll}1 & 1 \\2 & 3\end{array}\right]=\left[\begin{array}{cc}2 & 3 \\-1 & -2\end{array}\right]\left[\begin{array}{cc}1 & 1 \\2 & 3\end{array}\right]=\left[\begin{array}{cc}8 & 11 \\-5 & -7\end{array}\right]
\end{aligned}
$$




[επιστροφή στα περιεχόμενα](./README.md)
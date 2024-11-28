<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

# Κεφάλαιο 8 - Γραμμικά συστήματα

[επιστροφή στα περιεχόμενα](./README.md)




## Άσκηση 8.1

**Περιγραφή**

Να λυθεί το παρακάτω γραμμικό σύστημα εξισώσεων:

$$
\begin{align*}
    2x + 3y - z &= -3 \\
    4x - y + 2z &= -2 \\
    x + 2y + 3z &= 2
\end{align*}
$$

**Λύση**


Το σύστημα μπορεί να αναπαρασταθεί με την μορφή πινάκων $AX = B$, όπου

$$
A =
\begin{bmatrix}
    2 & 3 & -1 \\
    4 & -1 & 2 \\
    1 & 2 & 3
\end{bmatrix}
, \, \,
X =
\begin{bmatrix}
    x \\
    y \\
    z
\end{bmatrix}
, \, \,
B =
\begin{bmatrix}
    -3 \\
    -2 \\
    2
\end{bmatrix}
$$

Χρησιμοποιώντας την μέθοδο Κραμερ, μπορούμε να υπολογίσουμε τις τιμές των $x$, $y$, και $z$. Η λύση δίνεται από:

$$
x=\frac{D_x}{D}
, \, \,
y=\frac{D_y}{D}
, \, \,
z=\frac{D_z}{D}
$$

Υπολογίζουμε τις ορίζουσες:

$$
|D| = \begin{vmatrix}
    2 & 3 & -1 \\
    4 & -1 & 2 \\
    1 & 2 & 3
\end{vmatrix}
= 2(-3-4)-3(12-2)-1(8+1)
$$

$$
|D| = -14-30-9=-53
$$

$$
|D_x| = \begin{vmatrix}
    -3 & 3 & -1 \\
    -2 & -1 & 2 \\
    2 & 2 & 3
\end{vmatrix}
= -3(-3-4)-3(-6-4)-1(-4+2)
$$

$$
|D_x| = 21+30+2=53
$$

$$
|D_y| = \begin{vmatrix}
    2 & -3 & -1 \\
    4 & -2 & 2 \\
    1 & 2 & 3
\end{vmatrix}
= 2(-6-4)+3(12-2)-1(8+2)
$$

$$
|D_y| = -20+30-10 = 0
$$

$$
|D_z| = \begin{vmatrix}
    2 & 3 & -3 \\
    4 & -1 & -2 \\
    1 & 2 & 2
\end{vmatrix}
= 2(-2+4)-3(8+2)-3(8+1)
$$

$$
|D_z| = 4-30-27=-53
$$

Συνεπώς η λύση είναι:

$$
x = \frac{|D_x|}{|D|} = \frac{53}{-53}=-1
$$

$$
y = \frac{|D_y|}{|D|} = \frac{0}{-53}=0
$$

$$
z = \frac{|D_z|}{|D|} = \frac{-53}{-53}=1
$$

---

## Άσκηση 8.2

**Περιγραφή**

Να λυθεί το παρακάτω γραμμικό σύστημα εξισώσεων:

$$
\begin{align*}
    3x + y + 5z &= 0 \\
    x + 5y + z &= 10 \\
    3x + 2y + 4z &= 3
\end{align*}
$$


**Λύση**


Το σύστημα μπορεί να αναπαρασταθεί με την μορφή πινάκων $AX = B$, όπου

$$
A =
\begin{bmatrix}
    3 & 1 & 5 \\
    1 & 5 & 1 \\
    3 & 2 & 4
\end{bmatrix}
, \, \,
X =
\begin{bmatrix}
    x \\
    y \\
    z
\end{bmatrix}
, \, \,
B =
\begin{bmatrix}
    0 \\
    10 \\
    3
\end{bmatrix}
$$

Χρησιμοποιώντας την μέθοδο Κραμερ, μπορούμε να υπολογίσουμε τις τιμές των $x$, $y$, και $z$. Η λύση δίνεται από:

$$
x=\frac{D_x}{D}
, \, \,
y=\frac{D_y}{D}
, \, \,
z=\frac{D_z}{D}
$$

Υπολογίζουμε τις ορίζουσες:

$$
|D| = \begin{vmatrix}
    3 & 1 & 5 \\
    1 & 5 & 1 \\
    3 & 2 & 4
\end{vmatrix}
= 3(5 \cdot 4 - 2 \cdot 1) + 1(1 \cdot 4-3 \cdot 1) + 5(1 \cdot 2-3 \cdot 5)
$$

$$
|D| = 3(20-2) - 1 \cdot 1 + 5 \cdot (-13) = 54 - 1 -65 = -12 
$$

$$
|D_x| = \begin{vmatrix}
    0 & 1 & 5 \\
    10 & 5 & 1 \\
    3 & 2 & 4
\end{vmatrix}
= 0(20-2)-1(40-3)+5(20-15)
$$

$$
|D_x| = 0 -37 + 25 = -12
$$

$$
|D_y| = \begin{vmatrix}
    3 & 0 & 5 \\
    1 & 10 & 1 \\
    3 & 3 & 4
\end{vmatrix}
= 3(40-3)-0(4-3)+5(3-30)
$$

$$
|D_y| = 111 + 0 -135 = -24
$$

$$
|D_z| = \begin{vmatrix}
    3 & 1 & 0 \\
    1 & 5 & 10 \\
    3 & 2 & 3
\end{vmatrix}
= 3(15-20)-1(3-30)+0(2-15)
$$

$$
|D_z| = -15+27+0 = 12
$$

Συνεπώς η λύση είναι:

$$
x = \frac{|D_x|}{|D|} = \frac{-12}{-12} = 1
$$

$$
y = \frac{|D_y|}{|D|} = \frac{-24}{12} = 2
$$

$$
z = \frac{|D_z|}{|D|} = \frac{12}{-12} = -1
$$

## Άσκηση 8.3

**Περιγραφή**

Αν $\alpha^3 + \beta^3=1$ να βρεθεί ο αντίστροφος του πίνακα Α

$$
A=\left[\begin{array}{lll}\alpha & b & 0 \\ 0 & \alpha & b \\ b & 0 & \alpha\end{array}\right]
$$

**Λύση**


$$
\begin{aligned}
|A|=\left|\begin{array}{lll}
\alpha & b & 0 \\
0 & \alpha & b \\
b & 0 & \alpha
\end{array}\right| &=\alpha \cdot\left|\begin{array}{cc}
\alpha & b \\
0 & \alpha
\end{array}\right|-b\left|\begin{array}{cc}
0 & b \\
b & \alpha
\end{array}\right|=\\
&=\alpha^{3}+b^{3}=1
\end{aligned}
$$

$A_{11}=(-1)^{2}\left|\begin{array}{ll}\alpha & b \\ 0 & \alpha\end{array}\right|=\alpha^{2}$

$A_{21}=(-1)^{3}\left|\begin{array}{ll}b & 0 \\ 0 & \alpha\end{array}\right|=-\alpha b$

$A_{31}=(-1)^{4}\left|\begin{array}{ll}b & 0 \\ \alpha & b\end{array}\right|=b^{2}$

$A_{12}=(-1)^{3}\left|\begin{array}{ll}0 & b \\ b & \alpha\end{array}\right|=b^{2} $

$A_{22}=(-1)^{4}\left|\begin{array}{ll}\alpha & 0 \\ b & \alpha\end{array}\right|=\alpha^{2} $

$A_{32}=(-1)^{5}\left|\begin{array}{ll}\alpha & 0 \\ 0 & b\end{array}\right|=-\alpha b$

$A_{13}=(-1)^{4}\left|\begin{array}{ll}0 & \alpha \\ b & 0\end{array}\right|=-\alpha b $

$A_{23}=(-1)^{5}\left|\begin{array}{ll}\alpha & b \\ b & 0\end{array}\right|=b^{2} $

$A_{33}=(-1)^{6}\left|\begin{array}{ll}\alpha & b \\ 0 & \alpha\end{array}\right|=\alpha^{2}$

$$
A^{-1}=\frac{1}{|A|} \alpha d j A=\left[\begin{array}{ccc}
\alpha^{2} & -\alpha b & b^{2} \\
b^{2} & a^{2} & -\alpha b \\
-\alpha b & b^{2} & \alpha^{2}
\end{array}\right]
$$

---

## Άσκηση 8.4

**Περιγραφή**

Να δείξετε ότι ο πίνακας Α είναι αντιστρέψιμος και να
υπολογιστούν τα στοιχεία $\alpha_{14}$, $\alpha_{43}$ και $\alpha_{32}$ του πίνακα $A^{-1}$

$$
A=\left[\begin{array}{cccc}4 & 2 & 0 & -2 \\ 2 & 3 & 1 & 3 \\ 3 & -3 & 0 & 4 \\ 5 & -4 & 1 & 0\end{array}\right]
$$

**Λύση**



$$
|A|=\left|\begin{array}{cccc}4 & 2 & 0 & -2 \\2 & 3 & 1 & 3 \\3 & -3 & 0 & 4 \\5 & -4 & 1 & 0\end{array}\right| 
\stackrel{\Gamma_{2} : \Gamma_{2}-\Gamma_{4}}{=}
$$

$$
=\left|\begin{array}{cccc}4 & 2 & 0 & -2 \\-3 & 7 & 0 & 3 \\3 & -3 & 0 & 4 \\5 & -4 & 1 & 0\end{array}\right|=
$$

$$
=1 \cdot(-1)^{4+3} \cdot
\left|\begin{array}{ccc}
4 & 2 & -2 \\
-3 & 7 & 3 \\
3 & -3 & 4
\end{array}\right|
\underset{
\begin{subarray}{l}
\Sigma_{1}: \Sigma_{1}+2\Sigma_{3} \\ 
\Sigma_{2}: \Sigma_{2}+\Sigma_{3} 
\end{subarray}
}{=}
$$

$$
=-\left|
\begin{array}{ccc}
0 & 0 & -2 \\
3 & 10 & 3 \\
11 & 1 & 4
\end{array}
\right|= 
$$

$$
=-(-2)(-1)^4
\left|
\begin{array}{cc}
3 & 10 \\
11 & 1 
\end{array}
\right|= 
2(3-110)=-214
$$

$$
\alpha_{14}=\frac{1}{|A|} A_{41}=-\frac{1}{214}(-1)^{5}\left|\begin{array}{ccc}2 & 0 & -2 \\3 & 1 & 3 \\-3 & 0 & 4\end{array}\right|=\frac{1}{214}\left|\begin{array}{cc}2 & -2 \\-3 & 4\end{array}\right|=\frac{1}{107}
$$

$$
\alpha_{43}=\frac{1}{|A|} A_{34}=-\frac{1}{214}(-1)^{7}
\left|\begin{array}{ccc}
4 & 2 & 0 \\
2 & 3 & 1 \\
5 & -4 & 1
\end{array}\right|=
$$

$$
=\frac{1}{214}
\left|\begin{array}{ccc}
4 & 2 & 0 \\
-3 & 7 & 0 \\
5 & -4 & 1
\end{array}\right|=
\frac{1}{214}
\left|\begin{array}{cc}
4 & 2 \\
-3 & 7
\end{array}\right|
=\frac{17}{107}
$$

$$
\alpha_{32}=\frac{1}{|A|} A_{23}=-\frac{1}{214}(-1)^{5}\left|\begin{array}{ccc}4 & 2 & -2 \\3 & -3 & 4 \\5 & -4 & 0\end{array}\right|  
\stackrel{
\begin{subarray}{l}
\Sigma_{1}: \Sigma_{1}+2\Sigma_{3} \\ 
\Sigma_{2}: \Sigma_{2}+\Sigma_{3} 
\end{subarray}
}{=}
$$

$$
=\frac{1}{214}\left|\begin{array}{ccc}0 & 0 & -2 \\11 & 1 & 4 \\5 & -4 & 0\end{array}\right|=\frac{1}{214}(-2)\left|\begin{array}{cc}11 & 1 \\5 & -4\end{array}\right|=\frac{49}{107}
$$



---

## Άσκηση 8.5


**Περιγραφή**

Να υπολογιστεί η εξίσωση

$$
\left[\begin{array}{ll}2 & 1 \\3 & 2\end{array}\right] X \left[\begin{array}{cc}-3 & 2 \\5 & -3\end{array}\right]=\left[\begin{array}{cc}-2 & 4 \\3 & -1\end{array}\right] 
$$

**Λύση**


Οι πίνακες 

$$
\left[
\begin{array}{cc}
2 & 1 \\
3 & 2
\end{array}
\right] \quad , \quad
\left[
\begin{array}{cc}
-3 & 2 \\
5 & -3
\end{array}
\right]
$$

είναι αντιστρέψιμοι εφόσον

$$
\left|
\begin{array}{cc}
2 & 1 \\
3 & 2
\end{array}
\right|=1
\quad , \quad
\left|
\begin{array}{cc}
-3 & 2 \\
5 & -3
\end{array}
\right|=-1
$$

και οι αντίστροφοί τους είναι αντίστοιχα:

$$
\frac{1}{1}
\left[\begin{array}{cc}
2 & -1 \\
-3 & 2
\end{array}\right] 
\quad , \quad
\frac{1}{-1}\left[\begin{array}{ll}-3 & -2 \\-5 & -3\end{array}\right]\
$$



$$
\left[\begin{array}{cc}2 & 1 \\3 & 2\end{array}\right] X \left[\begin{array}{cc}-3 & 2 \\5 & -3\end{array}\right]=\left[\begin{array}{cc}-2 & 4 \\3 & -1\end{array}\right] 
$$

$$
\left[\begin{array}{ll}2 & 1 \\3 & 2\end{array}\right]^{-1} \left[\begin{array}{ll}2 & 1 \\3 & 2\end{array}\right]  X \left[\begin{array}{cc}-3 & 2 \\5 & -3\end{array}\right] \left[\begin{array}{cc}-3 & 2 \\5 & -3\end{array}\right]^{-1}=\left[\begin{array}{cc}2 & 1 \\3 & 2\end{array}\right]^{-1} \left[\begin{array}{cc}-2 & 4 \\3 & -1\end{array}\right] \left[\begin{array}{cc}-3 & 2 \\5 & -3\end{array}\right]^{-1}
$$

$$
I \cdot X \cdot I=\frac{1}{1}\left[\begin{array}{cc}2 & -1 \\-3 & 2\end{array}\right] \cdot\left[\begin{array}{cc}-2 & 4 \\3 & -1\end{array}\right] \frac{1}{-1}\left[\begin{array}{cc}-3 & -2 \\-5 & -3\end{array}\right]=\left[\begin{array}{cc}2 & -1 \\-3 & 2\end{array}\right] \cdot\left[\begin{array}{cc}-2 & 4 \\3 & -1\end{array}\right]\left[\begin{array}{cc}3 & 2 \\5 & 3\end{array}\right]
$$

$$
X=\left[\begin{array}{cc}-4-3 & 8+1 \\6+6 & -12-2\end{array}\right]\left[\begin{array}{cc}3 & 2 \\5 & 3\end{array}\right]=\left[\begin{array}{cc}-7 & 9 \\12 & -14\end{array}\right]\left[\begin{array}{cc}3 & 2 \\5 & 3\end{array}\right]
$$

$$
X=\left[\begin{array}{cc}-21+45 & -14+27 \\36-70 & 24-42\end{array}\right]=\left[\begin{array}{cc}24 & 13 \\-34 & -18\end{array}\right]
$$

**end comment**

---

## Άσκηση 8.6


**Περιγραφή**

Να λυθεί το σύστημα:

$$
\left.\begin{array}{l}
2 x_{1}-5 x_{2}-2 x_{3}-5 x_{4}=-1 \\
x_{1}-2 x_{2}-x_{3}-2 x_{4}=0 \\
3 x_{1}-5 x_{2}-2 x_{3}-3 x_{4}=1 \\
-x_{1}+4 x_{2}+4 x_{3}+11 x_{4}=2
\end{array}\right\}
$$

**Λύση**


Ακολοθούμε τη μέθοδο του $Gauss$ και σχηματίζουμε τον επαυξημένο πίνακα του συστήματος και έχουμε:

$$
\left[\begin{array}{cccc|c}
2 & -5 & -2 & -5 & -1 \\
1 & -2 & -1 & -2 & 0 \\
3 & -5 & -2 & -3 & 1 \\
-1 & 4 & 4 & 11 & 2
\end{array}\right] \stackrel{\Gamma_2 \leftrightarrow \Gamma_1}{\longrightarrow}
$$

$$
\left[\begin{array}{cccc|c}
1 & -2 & -1 & -2 & 0 \\
2 & -5 & -2 & -5 & -1 \\
3 & -5 & -2 & -3 & 1 \\
-1 & 4 & 4 & 11 & 2
\end{array}\right]
\underset{
\begin{subarray}{l}
\Gamma_2: \Gamma_2-2 \Gamma_1 \\
\Gamma_3: \Gamma_3-3 \Gamma_1 \\
\Gamma_4: \Gamma_4+\Gamma_1
\end{subarray}}{\longrightarrow}
$$

$$
\left[\begin{array}{cccc|c}
1 & -2 & -1 & -2 & 0 \\
0 & -1 & 0 & -1 & -1 \\
0 & 1 & 1 & 3 & 1 \\
0 & 2 & 3 & 9 & 2
\end{array}\right] \stackrel{\Gamma_2 \leftrightarrow \Gamma_3}{\longrightarrow}
$$

$$
\left[\begin{array}{cccc|c}
1 & -2 & -1 & -2 & 0 \\
0 & 1 & 1 & 3 & 1 \\
0 & -1 & 0 & -1 & -1 \\
0 & 2 & 3 & 9 & 2
\end{array}\right]
\underset{
\begin{subarray}{l}
\Gamma_3: \Gamma_3+\Gamma_2 \\
\Gamma_4: \Gamma_4-2 \Gamma_2
\end{subarray}}{\longrightarrow}
$$

$$
\left[\begin{array}{cccc|c}
1 & -2 & -1 & -2 & 0 \\
0 & 1 & 1 & 3 & 1 \\
0 & 0 & 1 & 2 & 0 \\
0 & 0 & 1 & 3 & 0
\end{array}\right] \stackrel{\Gamma_4: \Gamma_4-\Gamma_3}{\longrightarrow}
$$

$$
\left[\begin{array}{cccc|c}1 & -2 & -1 & -2 & 0 \\ 0 & 1 & 1 & 3 & 1 \\ 0 & 0 & 1 & 2 & 0 \\ 0 & 0 & 0 & 1 & 0\end{array}\right] \stackrel{\Gamma_1: \Gamma_1+2 \Gamma_2}{\longrightarrow}
$$

$$
\left[\begin{array}{llll|l}1 & 0 & 1 & 4 & 2 \\ 0 & 1 & 1 & 3 & 1 \\ 0 & 0 & 1 & 2 & 0 \\ 0 & 0 & 0 & 1 & 0\end{array}\right] 
\underset{
\begin{subarray}{l}
\Gamma_1: \Gamma_1-\Gamma_3 \\
\Gamma_2: \Gamma_2-\Gamma_3
\end{subarray}}{\longrightarrow}
$$

$$
\left[\begin{array}{llll|l}1 & 0 & 0 & 2 & 2 \\ 0 & 1 & 0 & 1 & 1 \\ 0 & 0 & 1 & 2 & 0 \\ 0 & 0 & 0 & 1 & 0\end{array}\right] 
\underset{
\begin{subarray}{l}
\Gamma_1: \Gamma_1-2\Gamma_4 \\
\Gamma_2: \Gamma_2-\Gamma_4 \\
\Gamma_3: \Gamma_3-2\Gamma_4
\end{subarray}}
{\longrightarrow}
$$


$$
\left[\begin{array}{llll|l}
1 & 0 & 0 & 0 & 2 \\
0 & 1 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0
\end{array}\right]
$$

Επομένως η λύση του συστήματος είναι (2,1,0,0)


---


## Άσκηση 8.7


**Περιγραφή**

Να λυθεί το σύστημα:

$$
\begin{array}{l}
(\lambda+2)x-y+(\lambda+1) w=0 \\
2 x+\lambda y+w=0 \\
\lambda x-3 y+\lambda w=0
\end{array}
\Rightarrow
$$

**Λύση**

$$
\Rightarrow
\left|\begin{array}{ccc}
\lambda+2 & -1 & \lambda+1 \\
2 & \lambda & 1 \\
\lambda & -3 & \lambda
\end{array}\right|
\underset{\Sigma_{1}=\Sigma_{1}-\Sigma_{3}}{=}
$$

$$=
\left|\begin{array}{ccc}
1 & -1 & \lambda+1 \\
1 & \lambda & 1 \\
0 & -3 & \lambda
\end{array}\right|
\underset{\Gamma_{1}=\Gamma_{1}-\Gamma_{2}}{=}
$$

$$
=\left|\begin{array}{ccc}
0 & -1-\lambda & \lambda \\
1 & \lambda & 1 \\
0 & -3 & \lambda
\end{array}\right|=
$$

$$
=(-1)^{3}\left|\begin{array}{cc}
-1-\lambda & \lambda \\
-3 & \lambda
\end{array}\right|=
$$

$$
=-(-\lambda - \lambda^2 + 3 \lambda)=
-(2\lambda -\lambda^2)=\lambda(\lambda-2)
$$

Η ορίζουσα μηδενίζεται για $\lambda=0$ ή $\lambda=2$. Αν $\lambda \neq 0$ και $\lambda \neq 2$ τότε το σύστημα έχει μοναδική λύση τη μηδενική (0, 0, 0)



Αν λ=0 το σύστημα γίνεται:

$$
\left.
\begin{array}{l}
2x-y+w=0 \\
2 x+w=0 \\
-3 y=0
\end{array}
\right\}
\Rightarrow \quad
\begin{array}{l}
x=-w/2\\
-3 y=0
\end{array}
$$

Επομένως το σύστημα έχει άπειρο πλήθος λύσεων
της μορφής (-κ/2, 0, κ)


Αν λ=2 το σύστημα γίνεται:

$$
\begin{array}{l}
4 x-y+3 w=0 \\
2 x+2 y+w=0 \\
2 x-3 y+2 w=0
\end{array}
$$

και σχηματίζουμε τον επαυξημένο πίνακα (ακολουθούμε τη μέθοδο $Gauss$)

$$
\left[
\begin{array}{ccc|c}
4 & -1 & 3 & 0 \\ 
2 & 2 & 1 & 0 \\ 
2 & -3 & 2 & 0
\end{array}
\right] 
\underset{\Gamma_{1}: (1/4)\Gamma_{1}}{\longrightarrow}
$$

$$
\left[
\begin{array}{ccc|c}
1 & -1 / 4 & 3 / 4 & 0 \\ 
2 & 2 & 1 & 0 \\ 
2 & -3 & 2 & 0
\end{array}
\right] 
\underset{
\begin{subarray}{l}
\Gamma_{2}: \Gamma_{2}-2\Gamma_{1} \\ 
\Gamma_{3}: \Gamma_{3}-2\Gamma_{1}
\end{subarray}
}{\longrightarrow}
$$

$$
\left[\begin{array}{ccc|c}
1 & -1 / 4 & 3 / 4 & 0 \\
0 & 5 / 2 & -1 / 2 & 0 \\
0 & -5 / 2 & 1 / 2 & 0
\end{array}\right] 
\underset{\Gamma_{2}: (2/5)\Gamma_{2}}{\longrightarrow}
$$

$$
\left[
\begin{array}{ccc|c}
1 & -1 / 4 & 3 / 4 & 0 \\
0 & 1 & -1 / 5 & 0 \\
0 & -5 / 2 & 1 / 2 & 0
\end{array}\right]
\underset{\Gamma_{3}: \Gamma_{3}+(5/2)\Gamma_{2}}{\longrightarrow}
$$

$$
\left[
\begin{array}{ccc|c}
1 & -1 / 4 & 3 / 4 & 0 \\ 
0 & 1 & -1/5 & 0 \\
0 & 0 & 0 & 0
\end{array}
\right] 
\underset{\Gamma_{1}: \Gamma_{1}+(1/4)\Gamma_{1}}{\longrightarrow}
$$

$$
\left[
\begin{array}{ccc|c}
1 & 0 & 4/5 & 0 \\
0 & 1 & -1/5 & 0 \\
0 & 0 & 0 & 0
\end{array}\right]
\Rightarrow
$$

$$
\begin{array}{l}
x=-(4/5)w \\
y=(1/5)w
\end{array}
$$


Επομένως το σύστημα έχει άπειρο πλήθος λύσεων της μορφής: $(-4\kappa/5, \kappa/5, \kappa)$




[επιστροφή στα περιεχόμενα](./README.md)
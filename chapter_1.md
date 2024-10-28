<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>


# Κεφάλαιο 1 - Συναρτήσεις

[Επιστροφή στην αρχική σελίδα](./README.md)

## Άσκηση 1.1

**Περιγραφή**

Να βρεθεί το σύνολο τιμών της συνάρτησης 
$ f(x)=\dfrac{x}{x+2}$

**Λύση**

$f(x)=\dfrac{x}{x+2}$ άρα πεδίο ορισμού το $(-\infty,-2)\cup(-2,+\infty)$.

Για την εύρεση του συνόλου τιμών αναζητούμε τις τιμές του $y$ για τις οποίες η $f(x)=y$ έχει λύση ως προς $x$ στο πεδίο ορισμού $(-\infty,-2)\cup(-2,+\infty)$.

$\dfrac{x}{x+2}=y \Rightarrow$

$x=yx+2y \Rightarrow$

$(1-y)x=2y \Rightarrow $

$x=\dfrac{2y}{1-y}$

* Για $y=1$, η εξίσωση είναι αδύνατη $0x=2$
*  Για $y=\neq 1$, η $x=\dfrac{2y}{1-y}$ έχει λύση στο $(-\infty,-2)\cup(-2,+\infty)$


Αν $x=-2 \Rightarrow $

$\dfrac{2y}{1-y}=-2 \Rightarrow $

$2y=-2+2y$ αδύνατο 

Επομένως το σύνολο τιμών είναι $f(A)=(-\infty,1)\cup(1,+\infty)$

---

## Άσκηση 1.2

**Περιγραφή** 

Να βρεθεί το σύνολο τιμών της συνάρτησης 
$f(x)=\dfrac{x^2 + x +4}{x^2-x+2}$

**Λύση**

$x^2-x+2=0 \Rightarrow$ 

$\Delta=(-1)^2 - 4\cdot2\cdot1 = 1-8=-7<0$.

 Άρα δεν υπάρχουν τιμές που να μηδενίζουν το πολυώνυμο.

Επομένως $x^2-x+2 \neq 0 \quad \forall x \in \mathbb{R}$, δηλαδή πεδίο ορισμού το $\mathbb{R}$.

Για την εύρεση του συνόλου τιμών αναζητούμε τις τιμές του $y$ για τις οποίες η $f(x)=y$ έχει λύση ως προς $x$ στο πεδίο ορισμού $\mathbb{R}$.

$f(x)=y \Rightarrow$ 

$\dfrac{x^2 + x +4}{x^2-x+2}=y \Rightarrow $ 

$x^2 + x +4=y(x^2-x+2) \Rightarrow$

$(1-y)x^2 + (1+y)x+4-2y=0$ (1)


* Αν $y=1$ τότε (1) $\Rightarrow 2x+4-2=0\Rightarrow x=-1$.  
Το $-1\in \mathbb{R}$ επομένως η $y=1 \in f(A)$.

* Αν $y\neq 1$ τότε (1) έχει λύση στο $\mathbb{R}$ αν $\Delta \geq 0$  
$\Rightarrow (1+y)^2 - 4(4-2y)(1-y) \geq 0$  
$\Rightarrow 1+y^2+2y-4(4-4y-2y+2y^2)\geq 0$  
$\Rightarrow 1+y^2+2y-16+24y-8y^2 \geq 0$  
$\Rightarrow -7y^2+26y-15 \geq 0$  
$\Rightarrow \frac{5}{7} \leq y \leq 3$  
$\Rightarrow f(A) = [ \dfrac{5}{7},3]$ περιλαμβάνει το $y=1$

---

## Άσκηση 1.3

**Περιγραφή**

Να βρεθεί το σύνολο τιμών της συνάρτησης 
$f(x)=\sqrt{1-x^2} + \sqrt{x^2-1}$

**Λύση**

* $1-x^2 \geq 0 \Rightarrow -1 \leq x \leq 1$
* $x^2-1 \geq 0 \Rightarrow x \leq -1 \; \kappa a \iota \; x\geq 1$

Συνεπώς πεδίο ορισμού $A=\{-1,1\}$

Για την εύρεση του συνόλου τιμών αναζητούμε τις τιμές του $y$ για τις οποίες η $f(x)=y$ έχει λύση ως προς $x$ στο πεδίο ορισμού $Α$.

$f(1)=f(-1)=0$ επομένως πεδίο τιμών $f(A)=0$

---

## Άσκηση 1.4

**Περιγραφή**

Να προσδιορίσετε τα κοινά σημεία των γραφικών παραστάσεων των $f(x)=x^2-3x+2$ και $g(x)=\dfrac{6}{x}$

**Λύση**

$f(x)=x^2-3x+2 \rightarrow$ πεδίο ορισμού $\mathbb{R}$

$g(x)=\dfrac{6}{x} \rightarrow$ πεδίο ορισμού $\mathbb{R}^*$

* $y = x^2-3x+2$ (1)
* $y = \dfrac{6}{x}$ (2)
 
(1),(2) $\Rightarrow \dfrac{6}{x} = x^2-3x+2 \Leftrightarrow $

$ \Leftrightarrow 6 = x^3 - 3x^2 + 2x$

$\Leftrightarrow x^3 - 3x^2 + 2x-6=0$

$\Leftrightarrow x^2(x-3) + 2(x-3)=0$

$\Leftrightarrow (x-3)(x^2+2)=0$

$\Leftrightarrow x=3$

Επομένως το σύστημα έχει λύση $(3,f(3))$ ή $(3,2)$ 

---

## Άσκηση 1.5

**Περιγραφή**

Να εξετάσετε αν ισχύει $f=g$, όπου $f(x)=\dfrac{x^2-5x+6}{x^2-4}$ και $g(x)=\dfrac{x-3}{x+2}$

**Λύση**

* $f(x)=\dfrac{x^2-5x+6}{x^2-4}=\dfrac{(x-2)(x-3)}{(x-2)(x+2)}=\dfrac{x-3}{x+2} \Rightarrow$ </br>
πεδίο ορισμού $(-\infty,-2)\cup(-2,2)\cup(2,+\infty)$

* $g(x)=\dfrac{x-3}{x+2} \Rightarrow$ πεδίο ορισμού $(-\infty,-2)\cup(-2,+\infty)$

Άρα $f(x)=g(x)$ στο $(-\infty,-2)\cup(-2,2)\cup(2,+\infty)$

---

## Άσκηση 1.6

**Περιγραφή**

Να εξετάσετε αν ισχύει $f=g$, όπου $f(x)=\dfrac{\sqrt{x-1}}{\sqrt{x}}$ και $g(x)=\sqrt{\dfrac{x-1}{x}}$

**Λύση**


* $f(x)=\dfrac{\sqrt{x-1}}{\sqrt{x}}=\sqrt{\dfrac{x-1}{x}}$ </br>
 Θα πρέπει $x-1 \geq 0$ και $x>0$. </br>
 Άρα $x \geq 1$ και $x>0$. </br>
 Συνεπώς το πεδίο ορισμού είναι το $[1,+\infty)$

* $g(x)=\sqrt{\dfrac{x-1}{x}}$.  </br>
Θα πρέπει $x \neq 0$ και $\dfrac{x-1}{x} \geq 0$ </br>
$\Rightarrow x(x-1) \geq 0$  </br>
$\Rightarrow x<0$ και $x\geq1$

Συνεπώς το πεδίο ορισμού είναι το $(-\infty,0)\cap[1,+\infty)$

Άρα $f(x)=g(x)$ στο $[1,+\infty)$

---

## Άσκηση 1.7

**Περιγραφή**

Αν $f(x)=x+5$ και $g(x)=|x|$ να βρείτε την $(g \circ f)(4)$

**Λύση**

$$g(x) = |x| = 
\left\{ \begin{aligned}
& -x, \; x<0  \\
& x, \; x \geq 0 \\
\end{aligned} \right.$$ 
Άρα το πεδίο ορισμού των $f(x), \; g(x)$ είναι το $\mathbb{R}$.

$$(g \circ f)(x) = |x+5| = 
\left\{ \begin{aligned}
& -x-5, \; x<0  \\
& x+5, \; x \geq 0 \\
\end{aligned} \right.$$ 
Άρα $(g \circ f)(4) = 4+5=9$

---

## Άσκηση 1.8

**Περιγραφή** -

Να βρεθεί η μονοτονία της συνάρτησης $f(x)=\dfrac{2}{x-1}$

**Λύση**

Πεδίο ορισμού $(-\infty,1)\cap(1,+\infty)$

* Για $x_1, x_2 \in (-\infty,1)$ και $x_1 < x_2$ τότε 
$x_1 -1 < x_2 -1$ </br>
$\Rightarrow \dfrac{1}{x_1-1} > \dfrac{1}{x_2-1}$ </br>
$\Rightarrow \dfrac{2}{x_1-1} > \dfrac{2}{x_2-1}$ </br>
$\Rightarrow f(x_1)>f(x_2)$ </br>
$\Rightarrow$ Γνησίως φθίνουσα

* Για $x_1, x_2 \in (1,+\infty)$ και $x_1 < x_2$ τότε 
$x_1 -1 < x_2 -1$ </br>
$\Rightarrow \dfrac{1}{x_1-1} > \dfrac{1}{x_2-1}$ </br>
$\Rightarrow \dfrac{2}{x_1-1} > \dfrac{2}{x_2-1}$ </br>
$\Rightarrow f(x_1)>f(x_2)$ </br>
$\Rightarrow$ Γνησίως φθίνουσα

* Για $x_1 \in (-\infty,1)$ και $ x_2 \in (1,+\infty)$ τότε $x_1 < x_2$ </br>
$\Rightarrow x_1 -1 < x_2 -1$ </br>
$\Rightarrow \dfrac{1}{x_1-1} < \dfrac{1}{x_2-1}$ </br>
$\Rightarrow \dfrac{2}{x_1-1} < \dfrac{2}{x_2-1}$ </br>
$\Rightarrow f(x_1)<f(x_2)$ </br>
$\Rightarrow$ Γνησίως αύξουσα

---

## Άσκηση 1.9

**Περιγραφή**

Να βρεθεί η μονοτονία της συνάρτησης 
$$f(x)=\left\{ \begin{aligned}
& x, \; x<0  \\
& x^2, \; x \geq 0 \\
\end{aligned} \right.$$

**Λύση**


* Για $x_1, x_2 < 0, \; x_1<x_2 \Rightarrow f(x_1) < f(x_2) \rightarrow$ Γνησίως αύξουσα
* Για $x_1, x_2 \geq 0, \; x_1<x_2 \Rightarrow x_1^2 < x_2^2 \Rightarrow f(x_1) < f(x_2) \rightarrow$ Γνησίως αύξουσα
* Για $x_1 < 0 < x_2 \Rightarrow x_1 < x_2^2 \Rightarrow f(x_1) < f(x_2) \rightarrow$ Γνησίως αύξουσα


[Επιστροφή στην αρχική σελίδα](./README.md)

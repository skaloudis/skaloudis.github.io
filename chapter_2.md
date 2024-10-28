# Κεφάλαιο 2

[επιστροφή στα περιεχόμενα](./README.md)


<div id='id-section-toc'/>

## Περιεχόμενα
- [Κεφάλαιο 2 - ΄Ορια Συναρτήσεων](#id-section2)
    - [Άσκηση 2.1](#id-section-2-1)
    - [Άσκηση 2.2](#id-section-2-2)
    - [Άσκηση 2.3](#id-section-2-3)
    - [Άσκηση 2.4](#id-section-2-4)
    - [Άσκηση 2.5](#id-section-2-5)
    - [Άσκηση 2.6](#id-section-2-6)
    - [Άσκηση 2.7](#id-section-2-7)
    - [Άσκηση 2.8](#id-section-2-8)
    - [Άσκηση 2.9](#id-section-2-9)


</br></br></br>

<div id='id-section-2'/>

# Κεφάλαιο 2 - ΄Ορια Συναρτήσεων



<div id='id-section-2-1'/>

## Άσκηση 2.1

**Περιγραφή**

Να βρεθεί η μονοτονία της συνάρτησης 
$f(x)=\frac{2}{x-1}$

**Λύση**

Πεδίο ορισμού $(-\infty,1)\cap(1,+\infty)$

* Για $x_1, x_2 \in (-\infty,1)$ και $x_1 < x_2$ τότε 
$x_1 -1 < x_2 -1$ 

$\Rightarrow \frac{1}{x_1-1} > \frac{1}{x_2-1}$

$\Rightarrow \frac{2}{x_1-1} > \frac{2}{x_2-1}$

$\Rightarrow f(x_1)>f(x_2) \rightarrow$ Γνησίως φθίνουσα

* Για $x_1, x_2 \in (1,+\infty)$ και $x_1 < x_2$ τότε 
$x_1 -1 < x_2 -1$ 

$\Rightarrow \frac{1}{x_1-1} > \frac{1}{x_2-1}$

$\Rightarrow \frac{2}{x_1-1} > \frac{2}{x_2-1}$

$\Rightarrow f(x_1)>f(x_2) \rightarrow$ Γνησίως φθίνουσα

<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-2'/>

## Άσκηση 2.2

**Περιγραφή** -

Αν $$f(x)=\frac{x^2 -2|x|}{2(x-2)} +2$$ να αποδειχθεί ότι $$\lim_{x\to2} f(x) = 3$$

**Λύση**

Πεδίο ορισμού: $\mathbb{R}-\{2\}$
$$x>0 \Rightarrow f(x)=\frac{x^2 -2|x|}{2(x-2)} + 2 = \frac{x^2 -2x}{2(x-2)} + 2 = \frac{x}{2} + 2$$
$$x \in (0,2) \cup (2,+\infty)$$ 
$$ \lim_{x\to2} f(x) = \lim_{x\to2} \left( \frac{x}{2} + 2 \right) = 3$$

<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-3'/>

## Άσκηση 2.3

**Περιγραφή**

Να βρεθεί το σύνολο τιμών της συνάρτησης 
$f(x)=\sqrt{1-x^2} + \sqrt{x^2-1}$

**Λύση**

* $1-x^2 \geq 0 \Rightarrow -1 \leq x \leq 1$
* $x^2-1 \geq 0 \Rightarrow x \leq -1 \; \kappa a \iota \; x\geq 1$

Συνεπώς πεδίο ορισμού $A=\{-1,1\}$

Για την εύρεση του συνόλου τιμών αναζητούμε τις τιμές του $y$ για τις οποίες η $f(x)=y$ έχει λύση ως προς $x$ στο πεδίο ορισμού $Α$.

$f(1)=f(-1)=0$ επομένως πεδίο τιμών $f(A)=0$

<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-4'/>

## Άσκηση 2.4

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

<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-5'/>

## Άσκηση 2.5

**Περιγραφή**

Να εξετάσετε αν ισχύει $f=g$, όπου $f(x)=\dfrac{x^2-5x+6}{x^2-4}$ και $g(x)=\dfrac{x-3}{x+2}$

**Λύση**

* $f(x)=\dfrac{x^2-5x+6}{x^2-4}=\dfrac{(x-2)(x-3)}{(x-2)(x+2)}=\dfrac{x-3}{x+2} \Rightarrow$ </br>
πεδίο ορισμού $(-\infty,-2)\cup(-2,2)\cup(2,+\infty)$

* $g(x)=\dfrac{x-3}{x+2} \Rightarrow$ πεδίο ορισμού $(-\infty,-2)\cup(-2,+\infty)$

Άρα $f(x)=g(x)$ στο $(-\infty,-2)\cup(-2,2)\cup(2,+\infty)$

<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-6'/>

## Άσκηση 2.6

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


<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-7'/>

## Άσκηση 2.7

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


<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-8'/>

## Άσκηση 2.8

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


<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">

<div id='id-section-2-9'/>

## Άσκηση 2.9

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


<font size=2> <em> Επιστροφή στα [Περιεχόμενα](#id-section-toc) </em> </font>
<hr size="20" color="blue">
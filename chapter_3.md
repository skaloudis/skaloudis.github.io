<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

# Κεφάλαιο 3 - Παράγωγος Συνάρτησης

[επιστροφή στα περιεχόμενα](./README.md)



## Άσκηση 3.1

**Περιγραφή**

Να βρεθεί η παράγωγος των συναρτήσεων στο $x_o$.

α) $f(x)=\ln x \quad , \; x_{0}=2$

β) $f(x)=\sqrt{x} \quad , \; x_{0}=4$

**Λύση**

α) 

$$f(x)=\ln x \Rightarrow f^{\prime}(x)=\frac{1}{x}  \Rightarrow f^{\prime}(2)=\frac{1}{2}$$

β)

$$f(x)=\sqrt{x} \Rightarrow$$

$$f^{\prime}(x)=\dfrac{1}{2 \sqrt{x}} \Rightarrow$$

$$f^{\prime}(4)=\frac{1}{2 \sqrt{4}}=\frac{1}{4}$$

---

## Άσκηση 3.2

**Περιγραφή**

Να βρεθεί η παράγωγος της συνάρτησης $f(x)=(x^2+1)lnx$ στο $x_o=1$

**Λύση**

$$ f(x)=\left(x^{2}+1\right) \ln x \Rightarrow $$

$$ f^{\prime}(x)=\left(x^{2}+1\right)^{\prime} \ln x+\left(x^{2}+1\right)(\ln x)^{\prime}= $$

$$ = 2 x \ln x+\left(x^{2}+1\right) \frac{1}{x}= $$

$$  = 2 x \ln x+\frac{x^{2}+1}{x} \Rightarrow $$

$$f^{\prime}(1)=2 \cdot 1 \ln 1+\frac{1+1}{1}=2 \cdot 0+2=2$$


---

## Άσκηση 3.3

**Περιγραφή**

Να βρεθεί η παράγωγος των συναρτήσεων

α) $ f(x)=\ln \left(x^{2}-1\right) $

β) $ f(x)=\sqrt{2 x^{2}-x+3} $


**Λύση**

α)

$$f(x)=\ln \left(x^{2}-1\right)$$

$$f^{\prime}(x)=\frac{1}{x^{2}-1}\left(x^{2}-1\right)^{\prime}=\frac{2 x}{x^{2}-1}$$

β)

$$ f(x)=\sqrt{2 x^{2}-x+3} $$

$$ f^{\prime}(x)=\left(\sqrt{2 x^{2}-x+3}\right)^{\prime}=\frac{1}{2 \sqrt{2 x^{2}-x+3}}\left(2 x^{2}-x+3\right)^{\prime}=\frac{4 x-1}{2 \sqrt{2 x^{2}-x+3}}$$

---

## Άσκηση 3.4

**Περιγραφή**

Να βρεθεί η παράγωγος των συναρτήσεων όπου ορίζεται

α) $f(x)=\sqrt[3]{x^{2}}+\sqrt{x^{3}}$

β) $f(x)=\sqrt[4]{(2 x-6)}$

**Λύση**

**α)** $f(x)=\sqrt[3]{x^2} + \sqrt{x^3}$ 

Πεδίο ορισμού $A=[0,+\infty]$

Αν $x \in(0,+\infty)$ τότε

$$ f^{\prime}(x)=\left(\sqrt[3]{x^{2}}+\sqrt{x^{3}}\right)^{\prime}=\left(x^{2 / 3}+x^{3 / 2}\right)^{\prime}=\frac{2 x^{-1 / 3}}{3}+\frac{3 x^{1 / 2}}{2}=\frac{2}{3 \sqrt[3]{x}}+\frac{3}{2} \sqrt{x} $$

Αν $x=0$ τότε

$$ \lim _{x \rightarrow 0^{+}} \frac{f(x)-f(0)}{x-0}=\lim _{x \rightarrow 0^{+}} \frac{x^{2 / 3}+x^{3 / 2}}{x}=\lim _{x \rightarrow 0^{+}} \frac{1}{\sqrt[3]{x}}+\lim _{x \rightarrow 0^{+}} \sqrt{x}=+\infty $$

Επομένως η $f$ δεν είναι παραγωγίσιμη στο $x_0=0$


**β)** 
$f(x)=\sqrt[4]{2 x-6} \Rightarrow 2x-6 \geq 0 \Rightarrow x \geq 3$ 

Συνεπώς πεδίο ορισμού το $A=[3,+\infty)$

Αν $x \neq 3$ τότε

$$f^{\prime}(x)=(\sqrt[4]{2 x-6})^{\prime}=\left[(2 x-6)^{1 / 4}\right]^{\prime}=\frac{1}{4}(2 x-6)^{-3 / 4} \cdot(2 x-6)^{\prime}=\frac{1}{4} \frac{1}{\sqrt[4]{(2 x-6)^{3}}} \cdot 2=\frac{1}{2 \sqrt[4]{(2 x-6)^{3}}}$$

Αν $x=3$ τότε 

$$\lim _{x \rightarrow 3^{+}} \frac{f(x)-t(3)}{x-3}=\lim _{x \rightarrow 3^{+}} \frac{\sqrt[4]{2 x-6}}{x-3}=\sqrt[4]{2} \cdot \lim _{x \rightarrow 3^{+}} \frac{\sqrt[4]{x-3}}{x-3}=\sqrt[4]{2} \cdot \lim _{x \rightarrow 3^{+}} \frac{1}{\sqrt[4]{(x-3)^{3}}}=\sqrt[4]{2} \cdot(+\infty)=+\infty$$

Επομένως η $f$ δεν είναι παραγωγίσιμη στο $x_0=3$

---

## Άσκηση 3.5

**Περιγραφή**

Να εξεταστεί ως προς τη μονοτονία η συνάρτηση

$$ f(x)=\frac{x}{1+x^{2}} $$

**Λύση**

$1+x^2 \neq 0$ ισχύει για κάθε $x \in \mathbb{R}$. 

Συνεπώς το πεδίο ορισμού είναι το $\mathbb{R}$.

Η $f$ είναι συνεχής ως ρητή συνάρτηση.



$$
f^{\prime}(x)=\left(\frac{x}{1+x^{2}}\right)^{\prime}=\frac{(x)^{\prime}\left(1+x^{2}\right)-x\left(1+x^{2}\right)^{\prime}}{\left(1+x^{2}\right)^{2}}=
$$

$$ =\frac{1+x^{2}-2 x^{2}}{\left(1+x^{2}\right)^{2}}=
\frac{1-x^{2}}{\left(1+x^{2}\right)^{2}}=
\frac{(1-x)(1+x)}{(1+x^2)^2} $$

Άρα $x_1=-1$ και $x_2=1$


$$
\begin{array}{c|ccccccc|}
x   & -\infty &                   &-1  &  &1 & &+\infty \\
\hline
f' &              & -                & 0 &+ & 0 &- &\\
\hline
f  &              & \searrow & | & \nearrow &| &\searrow &\\
\end{array}
$$

Επομένως η $f$ είναι γνησίως αύξουσα στο διάστημα $[-1,1]$ και γνησίως φθίνουσα στο διάστημα $(-\infty, -1]$ και στο $[1,+\infty)$

---

## Άσκηση 3.6

**Περιγραφή**

Να γίνει η μελέτη της συνάρτησης

$$
f(x)=\frac{x^{2}}{\sqrt{x+1}}
$$

**Λύση**

$x+1>0 \Rightarrow x>-1$, συνεπώς πεδίο ορισμού: $(-1,+\infty)$

Η συνάρτηση $f$ είναι συνεχής ως ρητή.


$$
f'(x)=\left( \frac{x^2}{\sqrt{x+1}} \right)' =
$$

$$
\frac{(x^2)' \sqrt{x+1} - x^2 (\sqrt{x+1})'}{(\sqrt{x+1})^2}=
\frac{2x\sqrt{x+1} -x^2 \frac{(x+1)'}{2\sqrt{x+1}}}{(\sqrt{x+1})^2}=
$$

$$
=\frac{2 x \sqrt{x+1}-\frac{x^{2}}{2 \sqrt{x+1}}}{x+1}=
\frac{4 x(x+1)-x^{2}}{2 \sqrt{x+1}(x+1)}=
$$

$$
=\frac{3 x^{2}+4 x}{2(x+1)^{3 / 2}}=
\frac{x(3 x+4)}{2(x+1)^{3 / 2}}
$$

Αναζητούμε τα τοπικά ακρότατα στις ρίζες της $f'(x)=0$ και τα σημεία όπου δεν υπάρχει η $f'(x)$

Τοπικά ακρότατα: 
* $f^{\prime}(x)=0 \Rightarrow x_{1}=0 \; , \; x_{2}=-4 / 3$. Το $x=-\frac{4}{3}$ δεν ανήκει στο πεδίο ορισμού της f, επομένως δεν αποτελεί τοπικό ακρότατο. 
* $x_{2}=-1$



$$
f^{\prime \prime}(x)=\left(\frac{3 x^{2}+4 x}{2(x+1)^{3 / 2}}\right)^{\prime}=
$$

$$
\frac{\left(3 x^{2}+4 x\right)^{\prime} 2(x+1)^{3 / 2}-\left(3 x^{2}+4 x\right) 2\left((x+1)^{3 / 2}\right)^{\prime}}{\left(2(x+1)^{3 / 2}\right)^{2}}
$$

$$
=\frac{(6 x+4) 2(x+1)^{3 / 2}-\left(3 x^{2}+4 x\right) 2 \frac{3}{2}(x+1)^{1 / 2}}{4(x+1)^{3}}=
$$

$$
=\frac{(6 x+4) 2(x+1) \sqrt{x+1}-\left(3 x^{2}+4 x\right) 3 \sqrt{x+1}}{4(x+1)^{3}} \Rightarrow 
$$

$$
f^{\prime \prime}(x)=\frac{(6 x+4) 2(x+1)-3\left(3 x^{2}+4 x\right)}{4(x+1)^{5 / 2}}=
$$

$$
\frac{12 x^{2}+12 x+8 x+8-9 x^{2}-12 x}{4(x+1)^{5 / 2}}=
$$

$$\frac{3 x^{2}+8 x+8}{4(x+1)^{5 / 2}}$$


$3 x^{2}-8 x+8=0 \Rightarrow \Delta=64-4 \cdot 8 \cdot 3=-32<0$

$f ' '(x)>0$

$(x+1)^{5 / 2}>0$

$$
\begin{array}{c|ccccc}
x & -1 & & 0 & &+\infty \\
\hline
f' & &- & 0& + &  \\
\hline
f'' & &+ & |& + &  \\
\hline
f & &\searrow & |&\nearrow &  \\
\hline
\end{array}
$$

Επομένως η $f$ είναι γνησίως φθίνουσα στο $(-1,0]$ και γνησίως αύξουσα στο $[0, +\infty)$.

Είναι κυρτή στο $(-1, +\infty)$.

Τοπικό Ελάχιστο στο x=0 με ελάχιστη τιμή το $f(0)=0$.

Για $x=0$, $f(0)=0$ επομένως το σημείο τομής με τους άξονες είναι το (0,0).


---

## Άσκηση 3.7

**Περιγραφή**
Να γίνει η μελέτη της συνάρτησης
$f(x)=x+\frac{1}{x}$

**Λύση**\\

Πεδίο ορισμού $\mathbb{R}^{*}$. 
Η $f$ είναι συνεχής.


$f(-x)=-x+\frac{1}{-x}=-f(x)$ 
Περιττή: συμμετρική ως προς $O(0,0)$ 

$f^{\prime}(x)=\left(x+\frac{1}{x}\right)^{\prime}=1-\frac{1}{x^{2}}=\frac{x^{2}-1}{x^{2}}=\frac{(x-1)(x+1)}{x^{2}}$


Τοπικά ακρότατα: $f'(x)=0 \Rightarrow x_1=-1 \; , x_2=1$

$f''(x)=\left(1-\frac{1}{x^{2}}\right)'=-\left(-2 x^{-3}\right)=\frac{2}{x^{3}}$

$$
\begin{array}{c|ccccccccc}
x   & -\infty &                   &-1  &  &0 & &1 & &+\infty \\
\hline
f' &   & +   & 0 &- & | &-  &0 & + & \\
\hline
f'' &   & -   & | &- & | &+  &| & + & \\
\hline
f  &              & \nearrow & | & \searrow &| &\searrow & | & \nearrow\\
\end{array}
$$


Η $f''(x)$ δεν ορίζεται στο $x_0=0$ επομένως το $x_0=0$ αλλάζει το πρόσημο της $f''$.

Επομένως η f είναι γνησίως αύξουσα στα $(-\infty,-1]$ και $[1, +\infty)$ και γνησίως φθίνουσα στα διαστήματα [-1,0) και (0,1]. 

Είναι κοίλη στο $(-\infty,0)$ και κυρτή στο $(0,+\infty)$. 

Τοπικό Μέγιστο στο x=-1 το f(-1)=-2 : (-1,-2) 

Τοπικό Ελάχιστο στο x=1 το f(1)=2 : (1,2) 

Το $x_0=0$ δεν αποτελεί σημείο καμπής εφόσον δεν ανήκει στο πεδίο ορισμού της $f$.




---

## Άσκηση 3.8

**Περιγραφή**

Να υπολογιστούν τα παρακάτω όρια

a. $\lim _{x \rightarrow 0} \frac{e^{x}-1}{x}$

b. $\lim _{x \rightarrow+\infty} \frac{\ln x}{x^{k}}$ για $k>0$


**Λύση**

a.  

$$\lim _{x \rightarrow 0} \frac{e^{x}-1}{x}=\lim _{x \rightarrow 0} \frac{\left(e^{x}-1\right)^{\prime}}{(x)^{\prime}}=\lim _{x \rightarrow 0} \frac{e^{x}}{1}=1 $$

b. 

$$\lim _{x \rightarrow+\infty} \frac{\ln x}{x^{k}}=
\lim _{x \rightarrow+\infty} \frac{(\ln x)^{\prime}}{\left(x^{k}\right)^{\prime}}
=\lim _{x \rightarrow+\infty} \frac{\frac{1}{x}}{k x^{k-1}}=
\lim _{x \rightarrow+\infty} \frac{1}{k x^{k}}=0
$$

---

## Άσκηση 3.9

**Περιγραφή**

Να υπολογιστεί το παρακάτω όριο

$$\lim _{x \rightarrow 0} \frac{4 \eta \mu x} {7x-2x^2}$$


**Λύση**

$$
\lim _{x \rightarrow 0} \frac{4 \eta \mu x} {7x-2x^2}=
\lim _{x \rightarrow 0} \frac{(4 \eta \mu x)'} {(7x-2x^2)'}=
\lim _{x \rightarrow 0} \frac{4 \sigma \upsilon \nu 4 x} {7-4x} = 
\frac{4 \sigma \upsilon \nu (4 \cdot 0)} {7-4 \cdot 0}=
\frac{4}{7}
$$

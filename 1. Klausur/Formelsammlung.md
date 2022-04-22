## 0. Rotation und Divergenz von E
Die folgenden Bedingungen müssen für jedes statische elektrische Feld $\boldsymbol{E}(\boldsymbol{x})$ gelten:
$$Rotation:\,\boldsymbol{\nabla}\times\boldsymbol{E}=\epsilon_{ijk}\cdot\partial_j\cdot E_k=0$$
$$Divergenz:\,\boldsymbol{\nabla}\cdot\boldsymbol{E}=\partial_j\cdot E_j=\frac{\rho}{\epsilon_0}$$

Der Vollständigkeit halber auch die Formel für den Gradienten:
$$Gradient:\,(\nabla g)_i=\partial_ig$$

---

## 1. Gauß'sches Gesetz
### Integralform
$$\oint_S\boldsymbol{E}\cdot d\boldsymbol{A}=\frac{1}{\epsilon_0}\cdot\int_V\rho(\boldsymbol{x})\cdot d^3x=\frac{Q_{enclosed}}{\epsilon_0}$$

---

## 2. Das elektrische Feld
### Allgemeine Zusammenhänge
$$U=s\cdot E$$$$F=q\cdot E$$$$E=-\nabla V$$
### Bedingungen für elektrisches Feld in Elektrostatik
$$\nabla\times E=0$$
$$\nabla\cdot E=\frac{\rho}{\epsilon_0}\implies Gauss'sches\,Gesetz$$
### Colulomb'scher Ausdruck für $\boldsymbol{E_i(x_m)}$
$$E_i(x_m)=\frac{1}{4\pi\cdot\epsilon_0}\cdot\int d^3x\cdot\frac{\rho(x_m)\cdot(x_i-x_i')}{{|x_m-x_m'|}^3}$$

### Dipolmoment
$$\vec{p}=\sum q_i\cdot\vec{r}_i$$
### Energie
Die Selbstenergie $U$ eines elektrischen Feldes $E$ ist:
$$U=\frac{\epsilon_0}{2}\cdot\int E^2\,d^3x$$

---

## 3. Poisson's Gleichung
$$-\nabla^2V=\frac{\rho}{\epsilon_0}$$

---

## 4. Das elektrische Potential
$$V(\boldsymbol{x})=\frac{1}{4\pi\cdot\epsilon_0}\cdot\int\frac{\rho(\boldsymbol{x'})}{|\boldsymbol{x}-\boldsymbol{x'}|}\,d^3x'$$
Ist das elektrische Feld bekannt, gilt für das elektrische Potential:
$$V(x)=-\int_{\Gamma}E\,dl$$
Das elektrische Potential entspricht dem Wegintegral von $x_0$ nach $x$.

---

## 5. Kugelkoordinaten
![[Kugelkoordinaten.png]]
$$\vec{r}(R,\theta,\varphi)=\left[{\begin{array}{cc} R\cdot\sin{\theta}\cdot\cos{\varphi} \\ R\cdot\sin{\theta}\cdot\sin{\varphi} \\ R\cdot\cos{\theta} \\ \end{array} }\right]$$
Bzw. mit einer anderen Parametrisierung:
$$\vec{r}(R,s,t)=\left[{\begin{array}{cc} R\cdot\sin{s}\cdot\cos{t} \\ R\cdot\sin{s}\cdot\sin{t} \\ R\cdot\cos{s} \\ \end{array} }\right]$$
In Kugelkoordinaten gilt:
$$dV=r^2\cdot\sin{\theta}$$
# @Andi: Stimmt das?
Zum Beispiel:
$$\int_VE\,dV=\int_0^R\int_0^{2\pi}\int_0^{\pi}E\,d\theta d\varphi dr=\int_0^R\int_0^{2\pi}\int_0^{\pi}E\cdot r^2\cdot\sin{\theta}\,dr=4\pi\cdot\int_0^RE\cdot r^2\,dr$$

---

## 6. Kreiskoordinaten / Polarkoordinaten
![[Polarkoordinaten.png]]
$$\vec{r}(R,\varphi)=\left[{\begin{array}{cc} R\cdot\cos{\varphi} \\ R\cdot\sin{\varphi} \\ \end{array} }\right]$$
Bzw. mit einer anderen Parametrisierung:
$$\vec{r}(s,t)=\left[{\begin{array}{cc} s\cdot\cos{t} \\ s\cdot\sin{t} \\ \end{array} }\right]$$

---

## 7. Zylinderkoordinaten
![[Zylinderkoordinaten.png]]
$$\vec{r}(R,\varphi)=\left[{\begin{array}{cc} R\cdot\cos{\varphi} \\ R\cdot\sin{\varphi} \\ \end{array} }\right]$$
Bzw. mit einer anderen Parametrisierung:
$$\vec{r}(s,t)=\left[{\begin{array}{cc} s\cdot\cos{t} \\ s\cdot\sin{t} \\ \end{array} }\right]$$
### Zylindersymmetrie
An den Deckflächen eines zylindersymmetrischen Systems ist $\vec{E}\bot dA$ . Daher sind diese für den Betrag des elektrischen Feldes irrelevant. ($\vec{E}=0$)

---

## 8. Integralsätze
![[Integralsätze.png]]
### Gaußscher Integralsatz
Der Satz von Gauß lautet für ein vom Rand $\partial V$ eingeschlossenes Volumen $V$ für ein beliebiges Vektorfeld mit den Komponenten $E_i$:
$$\int d^3V\partial_iE_i=\oint_{\partial V}dA_iE_i$$wobei $A_i$ die Komponenten des (stets nach außen gerichteten) Flächennormalvektors am Rand des Volumens sind.

### Stokescher Integralsatz
Der Satz von Stokes verknüpft ein Oberflächenintegral über eine (gekrümmte) Fläche mit einem Kurvenintegral über den Rand der Fläche:
$$\int_SdA_i\epsilon_{ijk}\partial_jF_k=\oint_{\partial S}ds_iF_i$$

---

## 9. Integrationsregeln
### Potenzregel
$$\int x^n\,dx=\frac{1}{n+1}\cdot x^{n+1}+C$$
### Faktorregel
$$\int c\cdot f(x)\,dx=c\cdot\int f(x)\,dx$$
### Summenregel
$$\int(f(x)+g(x))\,dx=\int f(x)\,dx+\int g(x)\,dx$$
### Differenzregel
$$\int(f(x)-g(x))\,dx=\int f(x)\,dx-\int g(x)\,dx$$
### Partielle Integration
$$\int f'(x)\cdot g(x)\,dx=f(x)\cdot g(x)-\int f(x)\cdot g'(x)$$
### Integration durch Substitution
$$\int f(x)\,dx=\int f(\varphi(u))\cdot\varphi'(u)\,du$$
### Besondere Regeln
$$\int\frac{1}{x}\,dx=\ln{(|x|)}+C$$

---

### 10. Ableitungsregeln
### Ableitung einer Konstanten
$$f(x)=C\rightarrow f'(x)=0$$
### Ableitung von x
$$f(x)=x\rightarrow f'(x)=1$$
### Potenzregel
$$f(x)=x^n\rightarrow f'(x)=n\cdot x^{n-1}$$
### Faktorregel
$$f(x)=c\cdot g(x)\rightarrow f'(x)=c\cdot g'(x)$$
### Summenregel
$$f(x)=g(x)+h(x)\rightarrow f'(x)=g'(x)+h'(x)$$
### Differenzregel
$$f(x)=g(x)-h(x)\rightarrow f'(x)=g'(x)-h'(x)$$
### Produktregel
$$f(x)=g(x)\cdot h(x)\rightarrow f'(x)=g'(x)\cdot h(x)+g(x)\cdot h'(x)$$
### Quotientenregel
$$f(x)=\frac{g(x)}{h(x)}\rightarrow f'(x)=\frac{h(x)\cdot g'(x)-g(x)\cdot h'(x)}{h^2(x)}$$
### Kettenregel
$$f(x)=g(h(x))\rightarrow f'(x)=g'(h(x))\cdot h'(x)$$
### Besondere Regeln
$$f(x)=\sqrt{x}\rightarrow f'(x)=\frac{1}{2\cdot\sqrt{x}}$$
$$f(x)=e^x\rightarrow f'(x)=e^x$$
$$f(x)=\ln{(x)}\rightarrow f'(x)=\frac{1}{x}$$
$$f(x)=\sin{x}\rightarrow f'(x)=\cos{x}$$
$$f(x)=\cos{x}\rightarrow f'(x)=-\sin{x}$$
$$f(x)=\tan{x}\rightarrow f'(x)=\frac{1}{\cos^2{x}}$$

---

## 11. Indexschreibweise
$$a\cdot b=a_i\cdot b_i$$
$$\vec{a}\times\vec{b}=\epsilon_{ijk}\cdot a_j\cdot b_k$$
$$\partial_ia_j=\delta_{ij}$$
$$\delta_{ij}\cdot a_i=a_j$$
$$\delta_{ij}\cdot\delta_{jk}=\delta_{ik}$$
$$\partial_ix_i=\delta_{ii}=n=3$$
$$\epsilon_{ijk}\cdot\epsilon_{klm}=det\left[{\begin{array}{cc} \delta_{il} & \delta_{im} \\ \delta_{jl} & \delta_{jm} \\ \end{array} }\right]=\delta_{il}\cdot\delta_{jm}-\delta_{jl}\cdot\delta_{im}$$
Das Levit-Civita-Symbol ändert unter Vertauschung zweier Indizes das Vorzeichen. z.B.:
$$\epsilon_{ijk}=-\epsilon_{jik}$$
$$\epsilon_{123}=1$$
$$\epsilon_{132}=-1$$
$$\epsilon_{122}=0$$

---

## 12. 


---

## 13. Allgemeine Rechenregeln
$$\hat{\boldsymbol{r}}=\frac{\vec{r}}{|r|}$$

---

## 14. Regel von de L’Hospital
Die Regel von de L’Hospital erlaubt es in vielen Fällen, den Grenzwert von Funktionen selbst dann noch zu bestimmen, wenn deren Funktionsterm beim Erreichen der betreffenden Grenze einen unbestimmten Ausdruck liefert. Zum Beispiel: $\frac{0}{0}$, $0\cdot\infty$,$\infty-\infty$,$\frac{\infty}{\infty}$,$0^0$,$\infty^0$,$1^{\infty}$

Die Regel von de L’Hospital besagt dann, dass, _falls_ der Grenzwert $\lim_{x\rightarrow x_0}\frac{f'(x)}{g'(x)}$ existiert, dieser zugleich der Grenzwert $\lim_{x\rightarrow x_0}\frac{f(x)}{g(x)}$ sei, wobei $f'(x)$ und $g'(x)$ hier die ersten Ableitungen der Funktionen $f(x)$ und $g(x)$ sein sollen.

## 15. Geometrische Formen
### Kreis
Umfang: $2\pi\cdot r$
Fläche: $r^2\cdot\pi$

### Zylinder
Mantelfläche: $2\pi\cdot r\cdot h$
Volumen: $r^2\cdot\pi\cdot h$

### Kugel
Oberfläche: $4\pi\cdot r^2$
Volumen: $\frac{4}{3}\cdot\pi\cdot r^3$



# TODO!!!
- Heaviside Funktion
- Dirac Funktion
- Wirbelfreiheit
- Maxwell-Gleichungen
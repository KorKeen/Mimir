---
tags:
---
## PDFs
- [Rektifikation Oldenburg](Rektifikation-Oldenburg_1735722931950_0.pdf)
- [PCVU Formeln](PCVU_Formeln_2304.pdf)

---
## Wichtige Formeln
### Trennfaktor / relative Flüchtigkeit
$$\alpha = \frac{p_A}{p_B}$$
$p_A$...Druck des leichter flüchtigen Stoffs
$p_B$...Druck von Stoff A

### Rücklaufverhältnis
$$r=\frac{\dot n_R}{\dot n_K}$$
$\dot n_R$...Stoffmengenstrom Rücklauf
$\dot n_K$...Stoffmengenstrom

### Verstärkergerade
$$y_D=\frac{1}{r+1}\cdot x_R+\frac{1}{r+1}\cdot x_K$$
$r$...Rücklaufverhältnis
$x_R$...Stoffmengenverhältnis Rücklauf
$x_K$...Stoffmengenverhältnis Kopf


### Abtriebsgerade
$$y_D=\frac{r'}{r'-1}\cdot x_R+\frac{r'}{r'-1}\cdot x_S$$
$r'$...Rückdampfverhältnis
$x_R$...Stoffmengenverhältnis Rücklauf
$x_S$...Stoffmengenverhältnis Sumpf

### Gleichgewichtskurve
$$y_A=\frac{x_A\cdot\alpha}{x_A \cdot(\alpha-1)+1}$$
$x_A$...Stoffmengenanteil A
$\alpha$...[Trennfaktor](((67692a2d-c051-4fab-a2c9-c782e36ece87)))

## Theorie
**Gleichgewichtsdiagramm:**
> Diese Methode basiert auf dem [McCabe–Thiele Verfahren](https://en.wikipedia.org/wiki/McCabe–Thiele_method) .

![[Gleichgewichtskurve-Rektifikation.svg | 400]]

Die <b style="color: gray;">ideale Gleichgewichtsgerade</b> symbolisiert keine Trennung und hat die Steigung $k=1$.

Stoffe lassen sich unterschiedlich gut trennen und benötigen verschieden aufwendige Rektifikationen. Als Maß dafür gibt es den [[#Wichtige Formeln#Trennfaktor / relative Flüchtigkeit | Trennfaktor]]. Aus diesem kann die [[#Wichtige Formeln#Gleichgewichtsgerade | Gleichgewichtskurve]] berechnet werden. 

Um herauszufinden wieviele Trennböden man benötigt werden muss man zwei Geraden einzeichnen:

<b style="color: green;">Verstärkergerade:</b>
Diese wird mittels dieser [[#Wichtige Formeln#Verstärkergerade | Formel]] berechnet. Diese Gerade beschreibt den Teil der Kolonne über dem Feed.
Sie verbindet die Kopfkonzentration auf der $y=x$ Gerade und die Feedkonzentration auf der Gleichgewichtsgerade bei einem Rücklauf von unendlich. Wenn Produkt entnommen wird muss die Gerade korrigiert werden.

<b style="color: red;">Abtriebsgerade:</b>
Diese wird mittels dieser [[#Wichtige Formeln#Abtriebsgerade | Formel]] berechnet und bezieht sich auf den Teil der Kolonne unter dem Feed.
Sie verbindet den Punkt an dem sich $x_F$ und die Verstärkergerade schneiden mit der Sumpfzusammensetzung auf der $y=x$ Gerade.

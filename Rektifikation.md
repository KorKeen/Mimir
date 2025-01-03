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
$$y_D=\frac{r}{r+1}\cdot x_R+\frac{1}{r+1}\cdot x_K$$
$r$...Rücklaufverhältnis
$x_R$...Stoffmengenverhältnis Rücklauf
$x_K$...Stoffmengenverhältnis Kopf


### Abtriebsgerade
$$y_D=\frac{r'}{r'-1}\cdot x_R-\frac{1}{r'-1}\cdot x_S$$
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


## Vorgehensweise Rechnen
**Beispiel 12.3:**
In einer kontinuierlich arbeitenden Gegenstromdestillationsanlage werden 1000 $kg/h$ eines Gemisches ($\alpha$ = 2,4), bestehend aus 25 Massen-% Benzol und 75 Massen-% Toluol, so getrennt, dass im Destillat 95 Massen-% Benzol und im Sumpf 98 Massen-% Toluol erhalten werden. Die Anlage arbeitet mit dem 2-fachen Mindestrücklaufverhältnis.
Der am Kopf der Kolonne angebrachte Kondensator arbeitet mit Totalkondensation ohne Temperaturabsenkung. Das Kühlwasser erwärmt sich dabei um 10 K.
Es sind zu berechnen:
a) Die theoretische Trennstufenzahl der Kolonne
b) Die benötigte Kühlwassermenge im Kondensator

$r_{mol,B} = r_B·M_B = 394 kJ·kg⁻¹ · 78,11 kg·kmol⁻¹ = 30775 kJ·kmol⁻¹$
$r_{mol,T} = r_T·M_T = 356 kJ·kg⁻¹ · 92,14 kg·kmol⁻¹ = 32802 kJ·kmol⁻¹$

**Schritte zur Berechnung**
1. Die Zusammensetzung des Kopfs und Feeds berechnen -> Stoffmengenverhältnis ($x_K$, $x_F$)
2. Das Gleichgewichtsdiagramm mit [[#Wichtige Formeln#Gleichgewichtskurve|Formel]] berechnen
3. Den $y$-Wert für den Feed berechnen
4. Das Mindestrücklaufverhältnis berechnen $$r_{min}=\frac{x_K-y_F}{y_F-x_F}$$
5. Für die Verstärkergerade die Werte berechnen $$y_D=r_{faktor}*x+d=\frac{r}{1+r}\cdot x+\frac{1}{1+r}\cdot x_K$$
   Dabei ist $$r_{fraktor}=\frac{r}{r+1}$$ $$d=\frac{1}{r+1}\cdot x_K$$
6. Das Diagramm sollte nun so ausschauen. ![[Pasted image 20250102130243.png|400]]
7. Tatsächlich wird jedoch ein höheres $r$ verwendet um Produkt abführen zu können. Also wird das $r_{theo}$ mit einem Faktor multipliziert und erneut berechnet. 
   $r_{faktor}$ und $d$ müssen erneut berechnet werden.
   
   Damit erhält man dieses Diagramm.
   ![[Pasted image 20250102131103.png|400]]
8. Nun wird die Abtriebsgerade berechnet mit dieser [[#Wichtige Formeln#Abtriebsgerade|Formel]] berechnet.
# Esimene ülesanne – Matemaatika trenažöör

**Ülesanded:**

* **Lisa juurde korrutamine ( * ) ja jagamine ( / )** arvu 100 piires, nii et 10x10 oleks suurim ja 100/___ kõrgeim jagamine. Jagamisel jagaja ja jagatava leidmiseks kasuta loogikat: 1 arv on 0 ... 10 ja teine arv on 1 ... 10 (<em>1 + random()*9</em>) ning küsi vastust tehtele:

```javascript
>arv_x * arv_y + " / " + arv_y
```
Selleks, et oleks võimalik loosida 2 ülesande asemel 4, on vaja juhuarvu loosimisel teha korrutus kolmega (loositavad arvud: 0, 1, 2, 3):

```javascript
Math.round(Math.random()*3)
```
* **Lisa juurde nupp** **Uus Ülesanne**.  Iga kord kui nupule vajutada loositakse uus tehe vana asemele ja tühjendatakse vastuse lahtri **value **atribuuti.
* **[VALIKULINE]** Võimalda funktsionaalsus, et lehe laadimisel on nupp **Uus Ülesanne **deaktiveeritud. Kui kasutaja vajutab nuppu **Kontrolli**, siis muuda see nupp mitteaktiivseks ning aktiveeri nupp Uus Ülesanne. Kui kasutaja vajutab nuppu Uus Ülesanne siis muuda see nupp mitteaktiivseks ning tee nupp Kontrolli aktiivseks. Nupu saad endale muutujana salvestada **init()** funktsiooni sees. **PS! Mõte seisneb selles, et me ei lase kasutajal uut ülesannet võtta enne kui eelmine on kontrollitud.**

```javascript
// lae nupp (tuleb teha init() funktsiooni käivitamise sees, sest siis on kindel, et nupp on olemas)
nupp = document.getElementById("nupp");
 
//dekativeeri
nupp.disabled = true
 
//aktiveeri
nupp.disabled = false;
```
* **Lisa juurde funktsioon `statistika();`**, mis arvutaks välja õigete vastuste protsendi ja kuvaks seda HTML'is **meter** elemendis **value** atribuudis. Õigete vastuste protsendi arvutamiseks tee tehe: **`P = õiged / kõik * 100`** (NB! Selleks, et seda meter elemendi value atribuudi sisse lisada peab see olema täisarv, tuleb ümardada!). Käivita statistika funktsiooni iga kord kui kasutaja kontrollib tehet.


Valmis lahendus laadimisel:

![alt text](https://raw.githubusercontent.com/veebirakenduste-kasutajaliidesed-2016k/matemaatika-trenazoor/master/matem_alg.png "Valmis lahendus laadmisel")

Valmis lahendus pärast juba mitmendat kontrollimist ja ühte vale tehet:

![alt text](https://raw.githubusercontent.com/veebirakenduste-kasutajaliidesed-2016k/matemaatika-trenazoor/master/matem_kontrollitud.png "Valmis lahendus pärast kontrollimist")

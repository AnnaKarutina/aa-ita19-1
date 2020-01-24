# 24.01
## Tunni teemad
### Järelkontrolliga tsükkel - `do while` tsükkel
```
do:
	//Siia kirjutame käsud, mida tuleb täita niikaua,
	//kui jätkamistingimus kehtib
while(jätkamistingimus)
```
Pange tähele, et täidetakse järelkontrolliga tsüklit alati vähemalt üks kord, sest jätkamistingimuse kontroll toimub alles pärast tsükli sisu täitmist.

### Tsüklite katkestamine - `break` ja `continue`
Tsükli kirjutamisel varitseb programmeerijat oht kirjutada tsükkel, mis töötab lõpmatult. Põhjus on selles, et kirjutati jätkamistingimus, mis alati jääb tõeseks, seda omakorda võib põhjustada sammu järeltegevuse ununemine (`for`-tsükli puhul on seda raskem unustada, sest järeltegevus kirjutatakse tsükli päisesse). Tsükli töö saab "pikema jututa" katkestada käsu `break` abil, mis suunab programmi täitmisjärje antud tsüklile järgnevale käsule.

Näide kasutamisest:
```
Integer summa = 0
Integer arv = 0
while (true)	//alati tõene, võib ka: for( ; ; )
	arv = arv + 1
	if (arv > 10) break // paneb tsükkel seisma, kui tingimus oleks täidetav
	summa = summa + arv
```

On olemas ka käsk `continue`, mis suunab programmi täitmisjärje tsükli järgmisele sammule, jättes antud sammul täitmata need käsud, mis jäid `continue` ja tsükli lõpu vahele

Kokkuvõtteks: 
* `break` peatab tsükli edaspidine töö täielikult
* `continue` laseb just antud samm vahele ja jätkab tegemist järgmisest sammust

### Kahekordsed tsüklid
Tsükli sisuks võib olla ka teine tsükkel.

Olgu meil näiteks vaja väljastada arvude 1, ..., 10 korrutustabel.

Oletame, et tühi tabel rea- ja veerunumbritega on juba olemas:
```
	x 1 2 3 4 5 6 7 8 9 10
	1
	2
	3
	4
	5
	6
	7
	8
	9
	10
```

Mõtleme, kuidas me tavaliselt toimime, kui hakkame tabelit täitma. Tõenäoliselt teeme seda reakaupa (või veerukaupa).

Niisiis, võtame ette 1. rea ja hakkame selle lahtritesse arvutuste tulemusi kirjutama. Vaatame 1. veeru kohal oleva arvu (1), korrutame reanumbri (1) sellega läbi ja kirjutame tulemuse (1) 1. rea ja 1. lahtrisse. 

Samuti toimime 2., 3., ..., 10. veeruga:
```
	x 1 2 3 4 5 6 7 8 9 10
	1 1 2 3 4 ...
```
Paneme tähele, et reanumber jäi kogu aeg samaks, aga veerunumber muutus ühest kümneni. See viib mõttele, et meil võiks olla "aeglane" tsükkel, mis teeb oma järgmise sammu alles siis, kui selle sees olev "kiire" tsükkel on kõik oma kümme sammu teinud.

Programmiga see võiks kuidagi nii olla kirjeldatud:
```
    for (int i = 1; i <= 10; i++):
	    for (int j = 1; j <= 10; j++):
		    Output(i * j & " ")
	    Output("reavahetus")
```

### Lisalugemist
* [Tsükkel](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/3-1-tsukkel/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks9`
* Salvesta antud kaustas kõik antud praktikumi programmid

### Ülesanne 1
Kirjutada programm, mis väljastab väljastab ekraanile järgmise kujundi:
```
* * * * * 
* * * * *
* * * * *
* * * * *
* * * * *
```

Salvesta fail nimega `ruut.fprg`

### Ülesanne 2
Täienda eelmine programm nii, et oleks võimalik määrata ruudus oleva ridade ja veergude arvu ka.

Salvesta fail nimega `ruut_muutuv.fprg`

### Ülesanne 3
Koosta programm, mis väljastab väljastab ekraanile järgmise kujundi:
```
* 
* * 
* * * 
* * * * 
* * * * *
``` 

Salvesta fail nimega `kolmnurk1.fprg`

### Ülesanne 4
Koosta programm, mis väljastab väljastab ekraanile järgmise kujundi:
```
* * * * *
* * * *
* * *
* * 
*
``` 

Salvesta fail nimega `kolmnurk2.fprg`

### Ülesanne 5
Täienda ülesanne 3 ka ridade numbrite näitamisega:
```
1 * 
2 * * 
3 * * * 
4 * * * * 
5 * * * * *
``` 
Salvesta fail nimega `kolmnurk3.fprg`

### Ülesanne 6
Täienda ülesanne 4 ka ridade numbrite näitamisega:
```
1 * * * * *
2 * * * *
3 * * *
4 * * 
5 *
``` 

Salvesta fail nimega `kolmnurk4.fprg`

### Ülesanne 7
Koosta programm, mis väljastab väljastab ekraanile järgmise kujundi:
```
        * 
      * * * 
    * * * * * 
  * * * * * * * 
* * * * * * * * * 
``` 

Salvesta fail nimega `kolmnurk5.fprg`

### Ülesanne 8
Täienda ülesanne 7 ka ridade numbri näitamisega:
```
1         * 
2       * * * 
3     * * * * * 
4   * * * * * * * 
5 * * * * * * * * * 
``` 

Salvesta fail nimega `kolmnurk6.fprg`

### Ülesanne 9
Koosta programm, mis väljastab väljastab ekraanile järgmise kujundi:
```
	* * * * * *
	*         *
	*         *
	*         *
	*         *
	* * * * * *
``` 

Salvesta fail nimega `raam.fprg`

### Ülesanne 10
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 11
Kopeeri `AA` kataloogs oleva `praks9` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
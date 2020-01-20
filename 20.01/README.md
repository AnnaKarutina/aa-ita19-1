# 20.01
## Tunni teemad
### Tsüklid - üldtsükkel (`for`) - teoreetiline materjal
Sageli on vaja, et mingeid direktiive täidetaks korduvalt. Seda saab realiseerida tsüklite abil.

<b>Põhistruktuur</b>
```
	for (eeltegevused; jätkamistingimus; sammu järeltegevused) 
		//käsud, mida tuleb täita niikaua,
		//kui jätkamistingimus kehtib
	
```
	
Tüüpiliselt on eeltegevusteks mingitele muutujatele algväärtuste omistamised. Võimalikud eeltegevused on näiteks järgmised:
```
    Integer i
    i = 0
```

Jätkamistingimus tuleb seada nii, et tsüklit täidetaks täpselt vajalik arv kordi. 

Näiteks kui soovime, et tsüklit täidetaks kolm korda, võib tsükli eeltegevusena omistada mingile lokaalmuutujale (tsükliloendajale) algväärtuseks nulli ja igal sammul liita tsükliloendajale ühe. Pärast tsükli esimest sammu on tsükliloendaja väärtus siis 1, pärast teist sammu 2 ja pärast kolmandat sammu 3. Neljandat sammu me enam lubada ei tohi, seega peaks tsükli lõpetama niipea, kui tsükliloendaja saab võrdseks 3-ga või 3-st suuremaks. Jätkamistingimus on lõpetamistingimuse vastandtingimus, ehk antud juhul võib tsüklit jätkata niikaua, kui tsükliloendaja on veel väiksem kolmest;

Olukorra kirjeldava for-tsükli päis on järgmine:
```
	for (int i = 0; i < 3; i = i + 1)
```

Tsükli sammu järeltegevuseks on sageli mingi muutuja väärtuse suurendamine või vähendamine teatud arvu võrra. Näiteks:
```
	i = i + 1;
	j = j + 2;
	k = k - 1;
```

Kirjutame näiteks for-tsükli, mis väljastab ekraanile viis korda teksti Tere!:
```
	for (int i = 0; i < 5; i++)
		Output("Tere!");
	
```

Lisalugemist
* [Tsükkel](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/3-1-tsukkel/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks7`
* Salvesta antud kaustas kõik antud praktikumi programmid

### Ülesanne 1
Koosta programm, mis väljastab esimese 10 täisarvu ruudud. Programm peab väljastama nii arvude väärtused kui ka ruutude väärtused.

Salvesta fail nimega `ruudud.fprg`

### Ülesanne 2
Kirjutada programm, mis väljastab esimese viie positiivse paaritu täisarvu ruudud. Programm peab väljastama nii arvude väärtused kui ka ruutude väärtused.

Salvesta fail nimega `paaritu_ruudud.fprg`

### Ülesanne 3
Kirjutada programm, mis arvutab esimese 10 täisarvu summa. Programm peab väljastama nii arvude väärtused kui ka jooksev ning lõplik summa väärtus.

Salvesta fail nimega `summa.fprg`
### Ülesanne 4
Kirjutada programm, mis arvutab esimese viie positiivse paaris täisarvu summa. Programm peab väljastama nii arvude väärtused kui ka summa väärtus.

Salvesta fail nimega `paaris_summa.fprg`
### Ülesanne 5
Olemas järgmine rida: 1, 3, 5, 7, ... Kirjutada programm, mis arvutab esimeste 10 rea liikme summa. Programm peab väljastama nii liikmete väärtused, kui ka lõpus nende summa väärtus.

Salvesta fail nimega `paaritu_summa.fprg`
### Ülesanne 6
Kirjutada programm, mis arvutab esimese ette antud arvu faktoriaal. Programm peab väljastama nii arvu väärtus, kui ka tema faktoriaali väärtus.

Salvesta fail nimega `faktoriaal.fprg`
### Ülesanne 7
Kirjutada programm, mis arvutab esimese 10 arvu faktoriaalid. Programm peab väljastama nii arvu väärtus, kui ka tema faktoriaali väärtus.

Salvesta fail nimega `faktoriaal10.fprg`
### Ülesanne 8
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 9
Kopeeri `AA` kataloogs oleva `praks7` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
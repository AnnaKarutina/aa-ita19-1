# 16.01
## Tunni teemad
### Tingimuslaused
Vahel on vaja eristada programmi täitmisel rohkem kui kahte haru. 

Seda saab realiseerida mitme tingimusdirektiiviga üksteise sees, näiteks:
```
	if (tingimus_1)
		if (tingimus_2)
			//tingimus_1 ja tingimus_2 on mõlemad täidetud
			direktiivid
		else
			//tingimus_1 on täidetud, aga tingimus_2 mitte
			direktiivid
	else
		//tingimus_1 ei ole täidetud (tingimus_2 ei mõju)
		direktiivid
```
Või teine võimalus, et tingimusdirektiivid on üks teisega seoses ja kontrollitakse üks teise järel, nagu ketti moodi:
```
    if (tingimus_1)
    {
        direktiiv_1;
        direktiiv_2;
        direktiiv_3;
    }
    else if (tingimus_2)
    {
        direktiiv_4;
        direktiiv_5;
    }
    else
    {
        direktiiv_6;
        direktiiv_7;
        direktiiv_8;
    }
```
### Loogilised tehted ja avaldised
[Loogilised operaatorid](https://github.com/AnnaKarutina/aa-ita19-1/tree/master/13.01)
Loogilised avaldised on võimalik moodustada mitte ainult tõeväärtuste abil, vaid kasutades ka tingimuslaused, mille tulemused ongi tõeväärtused. Näiteks 

`avaldis1 && avaldis2`

või

`avaldis1 || avaldis2`

Sellega tekkivad suuremad laused, kus kontrollitakse korraga mitu tingimust. 
Näiteks: `a > 0  && a < 5` võimaldab kontrollida, et a väärtus on vahemikust `(0; 5)` ehk ta peab olema rangelt suurem kui 0 ja rangelt väiksem kui 5. 
## Teoreetiline materjall
[Tingimuslause](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/tingimuslause/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks5`
* Salvesta antud kaustas kõik antud praktikumi programmid

### Ülesanne 1
Kirjutada programm, mis arvutab ruutvõrrandi lahendid. Tuleb omistada võrrandi kordajate väärtused, ülejäänud väärtused saadakse arvutamise kaudu. Juhul, kui omistatud väärtuste hulgas x<sup>2</sup> koefitsient on võrdne 0-ga, tuleb väljastada vastav teade.

Salvesta fail nimega `mata4.fprg`

### Ülesanne 2
Antud punkti koordinaadid x ja y (reaalarvud). Kirjutada programm, mis vastavalt etteantud punktile väljastab punktide koordinaatide väärtuseid ja kirjelduse, milles koordinaattasandi veerandis antud punkt paikneb. Kui punkt paikneb teljel, siis väljastatakse tekst "Antud punkt paikneb teljel." Programmi töö tulemus võib olla näiteks selline:

`Punkt koordinaatidega 2.0 ja 5.5 asub I veerandis.`

Salvesta fail nimega `mata5.fprg`

### Ülesanne X
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne XX
Kopeeri `AA` kataloogs oleva `praks5` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
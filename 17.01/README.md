# 17.01
## Tunni teemad
### Tingimuslaused - teoreetiline materjal
Võimalikud juhtumid
* [Tingimuslause tingimuslause sees](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/tingimuslause-tingimuslause-sees/)
* [Mitmeosaline tingimus. Loogilised tehted ja avaldised](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/mitmeosaline-tingimus-loogilised-tehted-ja-avaldised/)
* [Mitmeharuline tingimuslause](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/mitmeharuline-tingimuslause-elif-abil/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks6`
* Salvesta antud kaustas kõik antud praktikumi programmid

### Ülesanne 1
Täienda/muuda kehamassiindeksi ülesanne lahenduse nii, et sõltuvalt indeksi väärtusest oleks võimalik väljastada erinevad teated vastavalt tabelis toodud väärtuste vahemikutele:

Kategooria	| KMI vahemik
:---:|:---:
Tervisele ohtlik alakaal	| < 16
Alakaal	| 16 - 18.5
Normaalkaal	| 18.6 - 25
Ülekaal	| 25.1 - 30
Rasvumine	| 30.1 - 35
Tugev rasvumine	| 35.1 - 40
Tervisele ohtlik rasvumine	| > 40.1

Salvesta fail nimega `kmi2.fprg`

### Ülesanne 2
Kirjutada programm, mis arvutab ostuhinda arvestades ka allahindlust. Juhul kui ostu summa on suurem kui 50&euro;, allahindlus on 3%, juhul, kui ostu summa on suurem kui 100&euro;, allahindlus on 5%. Programm peab väljastama kõik väärtused koos kirjeldusega. Programmi töö tulemus võib olla näiteks selline:
```
	Ostu summa: 64€
	Saadav allahindlus on 3%
	Arvestades allahindlust osatu summa on: 62.80€
```

Salvesta fail nimega `ale.fprg`

### Ülesanne 3
Kirjutada programm, mis väljastab vastavalt kuu numbrile, millise sesooniga on tegemist. Programm peab väljastama kõik väärtused koos kirjeldusega. Programmi töö tulemus võib olla näiteks selline:
```
	Kuu number: 11
	Praegu on talv!
```
Salvesta fail nimega `kuu.fprg`
### Ülesanne 4
Koosta programm, mis etteantud täisarvu korral kontrollib, kas tegemist on paarisarvuga või paaritu arvuga, ja väljastab tulemus kujul:
```
   Arv 5 on paaritu
```
või
```
   Arv 8 on paaris
```
Salvesta fail nimega `paarsus.fprg`
### Ülesanne 5
Koosta programm, mis etteantud aastaarvu korrak kontrollib, kas tegemist [liigaastaga](https://et.wikipedia.org/wiki/Liigaasta) või mitte ja väljastab tulemus kujul.
```
    Aasta 2019 ei ole liigaasta.
```
või 
```
    Aasta 2020 on liigaasta.
```
Salvesta fail nimega `liigaasta.fprg`
### Ülesanne 6
Tutvu [Isikukoodi](https://et.wikipedia.org/wiki/Isikukood) struktuuriga. Deklareeri vastavad muutujad ning omista neile väärtused isikukoodi väärtusest. Näiteks kui isikukood on 49403136515, siis
```
    sugu = 4
    aasta = 94
    kuu = 3
```
jne.

Koosta prograam, mis kõigepealt kontrollib, et antud isikukood on kehtiv ning siis väljastab kõik vajalik info antud isikukoodiga inimesest - et ta on mees või naine, mis on tema sünnikuupäev kujul päev, kuu nimetus, aasta, kus ta on sündinud jne.

Salvesta fail nimega `id.fprg`
### Ülesanne 7
Koosta programm, mis kontrollib ette antud aasta numbri puhul, mitu päeva on antud aastal. Näiteks

```
    Aastal 2019 on 365 päeva.
```
<b>Vihje:</b>: Liigaastas on 366 päeva, tavaaastas aga 365. Lisaks olemas veel sajandid.

Salvesta fail nimega `paeva_arv_aastas.fprg`
### Ülesanne 8
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 9
Kopeeri `AA` kataloogs oleva `praks6` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
# 30.01
## Tunni teemad
### Järjendid - massiivid - näitena sõne
#### Sõne töötlus
Sõne töötlemisel või lähtuda sellest, et sõne tegelikult on massiivile sarnane andmetüüp, kus iga sümbol on võimalik saada kätte tema järjekorranumbri (indeksi) järgi. Indekseerimine analoogselt massiividega algab 0-st.
Näiteks 
```
    String tervitus = "Tere hommikust"
```
on võimalik käsitleda kui sümbolite massiiv:
```
    tervitus[0] = "T"
    tervitus[1] = "e"
    tervitus[2] = "r"
    tervitus[3] = "4"
    tervitus[4] = " "
    tervitus[5] = "h"
    tervitus[6] = "o"
    tervitus[7] = "m"
    tervitus[8] = "m"
    tervitus[9] = "i"
    tervitus[10] = "k"
    tervitus[11] = "u"
    tervitus[12] = "s"
    tervitus[13] = "t"
```
ja kui me soovime teada saada, mitu sümbolit on antud sõne sees olemas, siis seda saab üldiselt antud sõne ehk sümboli massiivi pikkuse abil teada saada.

### Tüübiteisendus funktsioonid Flowgorithm programmis
|funktsioon|kirjeldus|
|:---:|:---:|
`Char(s, i)` | teisendab sümboliks sone `s` sees oleva sümboli, mille indeks on `i`
`toInteger(a)` | teisendab sone `s` täisarvuks
`toString(n)` | teisendab sümboliks täisarvu `n`

### Rohkem teisendusfunktsioonidest
* [flowgorithm dokumentatsioon](http://www.flowgorithm.org/documentation/intrinsic-functions.htm)

### Lisalugemist
* [Sõned](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/soned/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks11`
* Salvesta antud kaustas kõik antud praktikumi programmid
### Ülesanne 1
Tutvu [Isikukoodi](https://et.wikipedia.org/wiki/Isikukood) struktuuriga. Programmi algus on niisugune:
<img src="http://anna.ikt.khk.ee/aa_ita19/29.01/id.png" width="700" alt="id.png">

Koosta programm, mille tulemus oleks:

`Antud id-ga inimene on mees/naine, kes on sündinud PP.KK.AAAA XXXXX haiglas ja tema id on ok`

Eeldused: 
* sugu saab tuvastada if lause abil
* vastavalt sugu numbrile saab AA juurde lisada vajalikud numbrid: 18 või 19 või 20 - if lause
* asukoht sama moodi saab if abil tuvastada
* id kontrolli astme kaalud on massiividena ning kontroll realiseerida for tsükli, tüübiteisenduse
  ja if lause abil 

Salvesta fail nimega `id_sone.fprg`

### Ülesanne 2
Koosta programm, mis küsib kasutaja käest tema ees ja perenimi ning nende põhjal moodustab kasutajanimi kujul `eesnimi.perenimi`. 

<b>Vihje: </b>
Sümbolite registri teisendamiseks võib kasutada tüübiteisendusfunktsiooni `toCode(symbol)` ning [ASCII](https://ascii.cl/) tabeli <i>decimal</i> väärtuste vahelist sõltuvust.

Salvesta fail nimega `kasutaja.fprg`
### Ülesanne 3
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 4
Kopeeri `AA` kataloogs oleva `praks11` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
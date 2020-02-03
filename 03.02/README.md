# 03.02
## Tunni teemad

---

### Funktsioonid
Funktsioonid kasutatakse programmi sisu organiseerimiseks ja korrastamiseks. Sisuliselt funktsioon on nimetatud algoritmi osa, millele kuuluvad käsud on mõeldud teatud probleemi lahendamiseks ja peavad sooritama oma tööd just kõik koos.

Siiamani oleme kasutanud olemasolevad funktsioonid - `Sqrt(number)`, `Char(string, index)`, `toInteger(string)` jne.

Aga juhul kui sobiva funktisooni ei eksisteeri, tuleb selle ise ära defineerida ja võta kasutusele.

#### Funktsiooni defineerimine
Funktsiooni defeneerimine on lihtne - tuleb määrata:
1. sobililik nimetus (see peaks olema loogiline, et oleks arusaadav, mille eest antud funktsioon vastutab)
2. parameetrite kogum - funktsioon on kinnine element - kui me soovime kasutada andmed väljaspoolt, siis tuleb kõigepealt need funktsiooni sisse edastada. Selleks kasutatakse funktsiooni `parameetrid`. Parameetrid on muutujad, mille kasutamine on võimalik ainult funktsioon sees - väljaspool funktsiooni nende väärtused ei ole kätte saadavad. Antud osa ei ole kohustuslik - olemas funktsioonid, mis ei vaja parameetreid enda töö jaoks.
3. funktsiooni sisu - käsklused, mis sooritakse antud funktsiooni kasutamisel.
4. tagastatav väärtus - kuna funktsioon on kinnine, siis kõik mis toimub selle sees, seal jääbki. Juhul, kui olemas soov funktisooni sisese tegevuse töö tulemus ka edaspidi kasutada, siis antud väärtus tuleb funktsiooni poolt tagastada - `return`.

Kokkuvõtteks:
```
    Define funktsiooniNimi(parameeter1, parameeter2, parameeter3, .. parameeterN)
        tegevused, mis peavad olema
        teostatud, kui kutsutakse antud funtksioon tööle
        tagastatav väärtus // viimane käsk, mis toimub funktisoonis
```
#### Näide - kasutaja tervitamine
Oletame, et meie ülesandeks tervitada kasutajat. Kui see peaks olema funktsiooni poolt realiseeritav, siis antud funktsioon tuleb defineerida:
<img src="http://anna.ikt.khk.ee/aa_ita19/03.02/01.png" width="900" alt="funktisooni defineerimine">
Antud juhul defineeritakse funktsioon nimega `tervitud`, mis ei oma veel ühtegi parameetrit ja ei tagasta mitte ühtegi väärtust. Sellise funktsiooni `return type` - tagastamistüüp - on `None`.

Nüüd on võimalik funktsioonile lisada ka sisemised käsklused:
<img src="http://anna.ikt.khk.ee/aa_ita19/03.02/02.png" width="500" alt="funktisooni defineerimine">
#### Funktsiooni kasutamine
Kui funktsioon on sisustatud - kasutamiseks tuleb <b>kutsuda</b> selle põhiprogrammis tööle:
 <img src="http://anna.ikt.khk.ee/aa_ita19/03.02/03.png" width="500" alt="funktisooni kutsumine">
 
  <img src="http://anna.ikt.khk.ee/aa_ita19/03.02/04.png" width="500" alt="funktisooni kutsumine">
 
 Ja tulemuseks:
 <img src="http://anna.ikt.khk.ee/aa_ita19/03.02/05.png" width="500" alt="funktisooni kutsumine">
#### Funktisooni parameetrid ja argumendid
Nüüd meie funktsioon tervitab kasutajat, aga mitte nimeliselt. Muudame funktsiooni definitsiooni nii, et oleks funktsioonil parameeter nimga `kasutajaNimi`, mille kaudu funktsioonile oleks võimalik edastada antud väärtus:
<img src="http://anna.ikt.khk.ee/aa_ita19/03.02/06.png" width="500" alt="funktisooni parameetrid">

Põhiprogrammis oleks nüüd vaja teisendada funktisooni kutsumise viis ning funktsiooni sees võta kasutusele parameeter:
<img src="http://anna.ikt.khk.ee/aa_ita19/03.02/07.png" width="500" alt="funktisooni parameetrid">

Tulemuseks on: 
<img src="http://anna.ikt.khk.ee/aa_ita19/03.02/08.png" width="500" alt="funktisooni parameetrid">

Antud juhul põhiprogrammis `"Kadi"` on `argument` - väärtus, mis edastatakse funktsioonile `parameetri` kaudu.

<b>Kokkuvõtte:</b>
* `parameeter` - muutuja, mille abil funktsiooni sisse on võimalik edastada väärtused - need me lisame siis, kui funktsioon nõuab parameetrite kaudu edastatud andmed oma töö sooritamiseks
* `argument` - muutuja, mille väärtus edastatakse funktsioonile parameetri kaudu või päris väärtus, mis sama moodi edastatakse parameetri kaudu siis, kui funktsioon kutsutakse tööle.
* kui kasutatakse rohkem kui 1 parameetreid - nende järjekord on väga oluline ja argumentide järjekord peab sellega ka kokku langema.
#### Tagastatavad väärtused - `return`
Kui on vajadus, et funktsiooni sees arvutatav tulemus oleks võimalik veel kuskil mujal väljaspoolt funktsiooni kasutada, siis see tuleb funktsioonist välja lükata - tagastada (inglise keeles `return`). Selleks kasutatakse samanimeline operaator. 

Antud operaator peab olema funktsiooni viimine operaator kuna pärast väärtuse tagastamist pole vajalik midagi veel teha.

Vastavalt sellele, millist tüüpi väärtus tagastab antud funktsioon, siis vastava funktsioon oleks ise täisarvuline, reaalarvuline, sõneline või boolean tüüpi funktsioon. Samuti on võimalik tagastada mitte ainult üksikud väärtused, aga terved väärtuste massiivid.

#### Näide - kahe punti vahekauguse arvutamine funktsiooni abil

Oletame, et olemas 2 punkti, mille koordinaadid on vastavalt `(x1, y1)` ja `(x2, y2)` , siis nende kahe punkti vaheline kaugus oleks:

<img src="http://anna.ikt.khk.ee/aa_ita19/03.02/09.png" width="500" alt="funktisooni väärtuse tagastamine">

#### Lisalugemist
* [Funktsioon](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/alamprogramm-funktsioon/)
* [Argumendid](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/argumendid-muutujad/)

### Ülesanded lahendamiseks
##### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks12`
* Salvesta antud kaustas kõik antud praktikumi programmid
##### Ülesanne 1
Täienda kasutaja tervitamise näide - valmista kasutajate nimede massiiv, mis koosneb vähemalt 5-st nimedest ning kõikide nende nimede jaoks kutsu `tervitus(kasutajaNimi)` funktsioon tööle.

Salvesta fail nimega `tervitus.fprg`

##### Ülesanne 2
Koosta funktsioon nimega `ringiPindala(ringiRaadius)`, mis võtab parameetrina ringiRaadiust (`Real` väärtusena) ning väljastab tulemusena lause: 
```
    Ringi raadiusega 5.78 pindala on 104.902376.
``` 
Kutsu funktsioon tööle ja kontrolli tulemus erinevate raadiuste väärtustega (võib rakendada tsükli, milles raadiusele määratakse juhuslik väärtus). 

Salvesta fail nimega `ringi_pindala.fprg`

##### Ülesanne 3
Koosta funktsioon nimega `kolmnurk(symbol)`, mis võtab parameetrina sümboli väärtus (`String` väärtusena) ning väljastab tulemusena kujundi, kui parameetrin edastatud sümboliks oli `*`: 
```
            * 
          * * * 
        * * * * * 
      * * * * * * * 
    * * * * * * * * * 
``` 
või 
```
        o 
      o o o 
    o o o o o 
  o o o o o o o 
o o o o o o o o o 
``` 
kui parameetrina edastatud sümboliks oli `o`.


Salvesta fail nimega `kujund1.fprg`

##### Ülesanne 4
Täienda ülesanne 3 lahendus nii, et funktsioonile oleks võimalik sisestada parameetrina nii kujundi sümbol kui ka ridade arv:
```
    * 
  * * * 
* * * * * 
``` 
või
```
        o 
      o o o 
    o o o o o 
  o o o o o o o 
o o o o o o o o o 
``` 

Salvesta fail nimega `kujund2.fprg`

##### Ülesanne 5
Koosta funktsioon nimega `summa(number)`, mis võtab parameetrina numbri (`Integer` väärtusena) ning arvutab kõikide numbrist väiksemate numbrite summat alates 1-st. Ehk kui `summa(10)` see tähendab et funktsioon arvutab `1 + 2 + 3 + ... + 10` ning tagastab arvutatud summa põhiprogrammile 

Salvesta fail nimega `summa.fprg`

##### Ülesanne 6
Koosta funktsioon nimega `taring`, mis tagastab kahe juhuslik täisarv (`Integer` väärtusena) vahemikust 1-6 summat.  Ehk kui visata `taring`, siis saab teada, palju oli siis kahe täringu summa antud vise korral. 

Salvesta fail nimega `taring.fprg`

##### Ülesanne 7
Koosta funktsioon nimega `paaris(number)`, mis võtab parameetrina täisarvu (`Integer` väärtusena) ning tagastab tõeväärtuse ehk `Boolean` tüüpi `true` kui number on paaris ja `false` kui number on paaritu.  Proovi 10 juhuslike täisarvude korral antud funktsiooni tööd. 

Salvesta fail nimega `paaris.fprg`

##### Ülesanne 8
Täienda ülesanne 7 programm - lisa funktsioon nimega `paaritu(number)`, mis oma tööde teostamiseks peab kasutama `paaris(number)` funktsiooni. Mõtle, kuidas see peaks toimuma algoritmiliselt.

Salvesta fail nimega `paaritu.fprg`

### Ülesanne 9
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 10
Kopeeri `AA` kataloogs oleva `praks12` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
# 07.02
## Tunni teemad

### Funktsioonid

#### Lisalugemist
* [Funktsioon](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/alamprogramm-funktsioon/)
* [Argumendid](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/argumendid-muutujad/)

### Ülesanded lahendamiseks
##### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks13`
* Salvesta antud kaustas kõik antud praktikumi programmid
##### Ülesanne 1
Kirjutada programm, mis sisaldab funktsiooni nimega `ruumala`, silindri ruumala arvutamiseks. Funktsiooni parameetrid on silindri raadius ja kõrgus. Funktsioon peab tagastama arvutatud väärtus ning põhiprogramm juba väljastab tulemus vastava kirjeldusega.

Salvesta fail nimega `silinder.fprg`

##### Ülesanne 2
Kirjutada programm, mis sisaldab funktsiooni nimega `ruutvorrand`. Antud funktsioon realiseerib ruutvõrrandi lahendamise. Funktsioon võtab argumentidena võrrandi kordajate väärtused ja tagastab vastavad täisarvud: 2 - võrrandil on 2 lahendid, 1 - voõrrandil on võrdsed lahendid, 0 - võrrandil puuduvad lahendid. Samuti juhul, kui esimene kordaja a on võrdne 0-ga, funktsioon tagastab -1.

Salvesta fail nimega `ruutvorrand.fprg`

##### Ülesanne 3
Koostage funktisoon nimega `kmindeks`, mis arvutab inimese massi ja pikkuse järgi kehamassiindeksi valemist `indeks = mass / (pikkus * pikkus)`. Mass on antud kilogrammides, pikkus meetrites.
Põhiprogrammis peavad mass ja pikkus saama juhuslikud väärtused (kasutage väärtused, mis võiksid täiskasvanud inimese puhul võimalikud olla). Põhifunktisoon peab rakendama kirjeldatud funktsiooni (kmindeks) koos seletava tekstiga väljastama inimese pikkuse, massi ja kehamassiindeksi. Kõik väärtused tuleb ümardada sajandikeni.

Salvesta fail nimega `kmi.fprg`

##### Ülesanne 4
Kirjutage programm, mis arvutab ja väljastab kolmnurga ümbermõõdu. Funktsioon nimega `vahemaa` peab arvutama külje pikkus, kasutades parameetritena kahe tipu koordinaadid. Põhiprogrammis tuleb punktide koordinaatidele esitavatele muutujatele omistada juhuslikud väärtused, mis on reaalarvud, ümardatud kümnendikeni;
ekraanile tuleb väljastada kolmnurga tippude koordinaadid, külgede pikkused ja ümbermõõt koos selgitava tekstiga.

Salvesta fail nimega `kolmnurk.fprg`

##### Ülesanne 5
Koostage programm, mis modelleerib täringu viskamist ja väljastab silmade arvu koos märkusega, kas see on paaris või paaritu.
Paarsuse kontrollimiseks koosta funktsioon nimega `paaris`, mis võtab parameetrina arvu ja tagastab true kui arv on paaris ning false kui on paaritu. 
Koostage funktsioon `taringuvise`, mis tagastab juhusliku täisarvu 1, 2, 3, 4, 5 või 6.

Põhiprogrammis vastavad funktisoonid rakendatakse ja väljastage tulemused koos seletava tekstiga.

Salvesta fail nimega `taring.fprg`

##### Ülesanne 6
Kausitäis paprikasuppi jahtub minuti jooksul 19% võrra suppi ja ruumi temperatuuride vahest. Koostage funktsioon, mille parameetrid on toatemperatuur ja suppi algtemperatuur. Antud funktsioon peab väljastama supi temperatuuri minutiliste ajavahemike tagant, samuti ka toa ja supi algtemperatuuri väärtused.
Näiteks toatemperatuur on 20 kraadi, supi algtemperatuur on 90 kraadi.
Põhiprogrammis rakendage teie poolt kirjutatud funktsioon.

Salvesta fail nimega `supp.fprg`

### Ülesanne 7
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 10
Kopeeri `AA` kataloogs oleva `praks13` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
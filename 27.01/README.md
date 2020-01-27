# 27.01
## Tunni teemad
### Järjendid - massiivid - näitena arvujärjend
#### Arvujärjendi loomine
Järjend aitab koondada teatavas mõttes ühetaolisi või ühesuguse tähendusega väärtusi ühte kohta. 
Niisugusteks väärtusteks võivad olla õhutemperatuurid järjestikustel päevadel, ühes rivis seisvate sõdurite pikkused vms. 
Näiteks viieliikmeline järjend a koosneb elementidest:
```
a[0]
a[1]
a[2]
a[3]
a[4]
```
Kõik elemendid on ühte ja sama tüüpi, arvu nurksulgudes (järjekorranumbrit) nimetatakse elemendi indeksiks. Iga element võib sõltumata teistest elementidest sisaldada korraga ühte väärtust - täisarvujärjendi puhul täisarvu, reaalarvujärjendi puhul reaalarvu jne, ning igale elemendile võib väärtuse omistada teisest elementidest sõltumatult.
Üldiselt kehtib reegel, et järjendi elementide numeratsioon algab alati nullist. Kui järjendis on kokku `n` elementi, siis viimase elemendi indeks on `n-1`.
Järjendi kirjeldamiseks (programmis kasutuselevõtmiseks) on mitu võimalust, kõige lihtsam on seda teha massiivialgati abil. 

Näiteks kui oleme viiel päeval lugenud kraadiklaasilt temperatuuri väärtused:
```
10     9     12     11     8
```
Siis võime nendest moodustada järjendi:
```
Integer[] a = {10, 9, 12, 11, 8}
```
Niisuguse kirjelduse toimel võetakse kasutusele täisarvujärjendi a ja omistab sellele elementidele järjestikku loogilistes sulgudes antud väärtused (seega näiteks `a[0]` väärtuseks saab `10` ja `a[1]` väärtuseks on `9`).
Ühtlasi määratakse kindlaks järjendi elementide arv ehk massiivi pikkus - praegusel juhul on selleks 5.

Teine võimalus järjendi kasutuselevõtuks on massiiviloome. Eelneva näitega samaväärse tulemuse saame ka nii, et moodustame kõigepealt käsuga:
```
Integer [] a = new Integer[5]
```

tühja viieelemendilise järjendi. Selle kõigi elementide algväärtuseks määratakse automaatselt 0.

Seejärel omistatakse elementidele nullide asemel vajalikud väärtused:
```
a[0] = 10;
a[1] = 9;
a[2] = 12;
a[3] = 11;
a[4] = 8;
```
Järjendi ühe elemendi väärtus võib väljastada standardsel viisil nagu iga teise muutuja väärtust. Näiteks korraldus:
```
Output("Jarjendi esimene element on " & a[0]);
```
väljastab ekraanile järjendi `a` esimese elemendi väärtuse

#### Näide arvujärjendi loomisest ja töötlemisest
<img src="http://anna.ikt.khk.ee/aa_ita19/27.01/naide1.PNG" width="500" alt="absoluutvaartus.png">

### Lisalugemist
* [Järjend](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/jarjend/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks10`
* Salvesta antud kaustas kõik antud praktikumi programmid

### Ülesanne 1
Antud 10-elemendiline täisarvude massiiv, mis sisaldab ka 0-lid. Programm väljastab nii elementide väärtused kui ka mittenulliliste elementide arvu.

Salvesta fail nimega `jarjend1.fprg`

### Ülesanne 2
Samasuguse massiiviga teostada järgmist: programm peab arvutama mittenulliliste elementide keskmise ja väljastada nii elementide väärtused kui ka mittenulliliste elementide indeksid ja keskmise.

Salvesta fail nimega `jarjend2.fprg`

### Ülesanne 3
Pankur on paigutanud oma raha 8 firmasse. Nädala lõpus saadab sekretär talle kokkuvõtte, kus on kirjas kuidas muutus iga firma aktsia hind selle nädala jooksul: kui palju tõusis või langes. Andmed on salvestatud 8-elemendilise massiivi, positiivne väärtus tähendab tõusu. Olemas ka massiiv, kus on salvestatud firmade nimed, mis on samuti 8-elemendiline. Järgmisel nädalal soovib pankur suurendada oma positsiooni kõigis neis firmades, mille aktsia sel nädalal odavnes. Kirjutada programm, mis väljastab kõikide selliste firmade nimed ja vastavad aktsia muutused.

Salvesta fail nimega `jarjend3.fprg`

### Ülesanne 4
Mööda konveierit liiguvad detailid. Konveieri kohale on paigutatud kaks läbivalgustusseadet, mis pärinevad erinevatest aastatest ja on erineva jõudlusega. Esimene seade vaatab läbi iga teise detaili ning teine seade iga kolmanda detaili. Tööpäeva alguses pannakse konveier käima ja tööpäeva lõpus, pärast n-nda detaili läbilaskmist, peatakse. Esimese detaili vaatavad läbi mõlemad seadmed. Mitu protsenti kõigist detailidest saab niimoodi läbi valgustatud ja mitu protsendi lipsab valgustamata läbi?

Näide: oletame, et tööpäeva jooksul vaadati läbi 12 detaili, tähistame need lihtsuse mõttes arvuga 0 kuni 11:
```
	detailid konveierilt 0	1	2	3	4	5	6	7	8	9	10	11
	1. seade valgustab   +		+		+		+		+		+	
	2. seade valgustab   +			+			+			+			
```
Seega vaadati 12 detailist läbi 8 ehk 66.7%, vaatamata jäi 4 ehk 33.3%.

Salvesta fail nimega `jarjend4.fprg`

### Ülesanne 5
Koosta programm, mis väljastab esialgse järjendi ning teisendab kõik järjendi elemendid vastupidiseks.

Salvesta fail nimega `jarjend5.fprg`

### Ülesanne 6
Koosta programm, mis järjendi kõige suurem ja kõige väksema väärtusega elemendid, ning väljastab nii nende väärtused kui ka indeksid.

Salvesta fail nimega `jarjend6.fprg`

### Ülesanne 7
Koosta programm, mis aitab lastel treenida liitmist. Programm peaks pakkuma välja juhuslike arvudega liitmistehteid ning ootama kasutajalt vastust. Kui vastus on õige, kiitma kasutajat, kui aga vale, andma õige vastuse ja esitama uue tehte. Järjest esitatavate tehete hulk võib olla programmis ette antud (näiteks 10), samuti võib olla ette antud piirid, kui suuri arve
kasutajalt küsitakse (näiteks 1 kuni 50). Programm peaks pidama arvestust ka õigete vastuste üle ning väljastama pärast viimast tehet tulemuse. 

Muutke programmi selliselt, et kasutajalt küsitakse ka teisi tehteid (lahutamine, korrutamine, jagamine). Tehte võite küsida kasutajalt või lasta arvutil genereerida erinevad tehted iga arvutuse kohta.

Muutke programmi nii, et esitavate arvude piirid saab kasutaja ette anda – nii maksimumi kui ka miinimumi.

Salvesta fail nimega `mata_mang.fprg`

### Ülesanne 8
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 8
Kopeeri `AA` kataloogs oleva `praks10` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
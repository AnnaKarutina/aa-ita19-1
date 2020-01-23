# 23.01
## Tunni teemad
### Tsüklid - eelkontrolliga tsükkel (`while`) - teoreetiline materjal
Sageli on vaja, et mingeid direktiive täidetaks korduvalt. Seda saab realiseerida tsüklite abil.

<b>Põhistruktuur</b>

```
    eeltegevused
	while (jätkamistingimus) 
		//käsud, mida tuleb täita niikaua,
		//kui jätkamistingimus kehtib
        //sammu järeltegevused
	
```
	
Lisalugemist
* [Tsükkel](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/3-1-tsukkel/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks8`
* Salvesta antud kaustas kõik antud praktikumi programmid

### Ülesanne 1
Kirjutada programm, mis väljastab esimese 10 positiivse täisarvu summa ja keskmine. Programm peab väljastama nii arvude väärtused kui ka summa ja keskmise väärtused. Lahendus peab olema realiseeritud while tsükli abil.

Salvesta fail nimega `summa_keskmine.fprg`

### Ülesanne 2
Antud arvud 1-st kuni 20-ni. Kirjutage programm, mis kontrollib, kas iga arv antud vahemikus on algarv või mitte. Programmis peab olema rakendatud while tsükkel.

Salvesta fail nimega `algarv.fprg`

### Ülesanne 3
Koosta programm, mis etteantud täisarvu korral arvutab antud arvu numbrite summat. Näiteks on antud ette arv `123`, siis programm suudab leida, et `1 + 2 + 3` on `6`. Programm peab töötama suvalise täisarvuga, ka negatiivse väärtusega. Sõnetöötlust kasutada ei tohi, ainult numbriliselt.

<b>Vihje</b>: püüa lahendada mitte `1 + 2 + 3` kujul vaid `3 + 2 + 1` kujul. 

Salvesta fail nimega `arvude_summa.fprg`

### Ülesanne 4
Koosta programm, mis leiab kõige suurem number arvu sees. Näiteks kui arv on `695`, siis programm tuvastab, et suurem number on `9`.

Salvesta fail nimega `suurem_number.fprg`

### Ülesanne 5
Koosta mäng, kus saate ära arvata arvuti poolt mõeldud täisarvu ühest viiekümneni. Programm peab töötama seni kuni õige arv on leitud ning teavitama sellest kasutajat.

Täienda programmi nii, et vale arvu sisestamisel antakse kasutajale vihje, kas arvuti poolt valitud arv on suurem või väiksem kasutaja sisestatud arvust.

Täienda programmi selliselt, et kui õige vastuse ja kasutaja sisestatud arvu vahe on väiksem või võrdne 5-ga, siis teavitatakse kasutajat, et ta on õigele vastusele juba üsna lähedale jõudnud.

Juhuarvu loomiseks kasuta funktsiooni `Random(arv)`, mis annab juhuslik väärtus `0` vahel `(arv-1)`.

Salvesta fail nimega `arvude_mang.fprg`
### Ülesanne X
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne XX
Kopeeri `AA` kataloogs oleva `praks8` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
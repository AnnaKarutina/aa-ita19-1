# 14.01
## Tunni teemad
### Tõeväärtused
- `Boolean` tüüpi väärtused
- `true` - tõene
- `false` - väär

### Võrdlus operaatorid:

|operaator|sümbol|
|:---:|:---:|
võrdub|`==`|
ei võrdu |`!=`|
suurem|`>`|
väiksem|`<`|
suurem võrdub|`>=`|
väiksem võrdub|`<=`|

### Tingimuslause 

* Kõikides eelnevates praktikumides koostasime programme, mille operaatorid (direktiivid) täideti üksteise järel, alates programmi algusest (esimesena kirja pandud operaatorist (direktiivist)) kuni lõpuni.
 
* On olemas palju ülesandeid, mida sellel viisil pole võimalik lahendada, käesolevas praktikumis vaatleme niisuguseid näiteid. Tingimusoperaatori (tingimusdirektiivi) abil saab vastavalt andmete korrektsetele väärtustele programmi täitmise kulgu suunata.

* Tingimusdirektiivi üldine kuju on
```
if (loogiline avaldis) 
    direktiiv_1 - täidetakse kui loogiline avaldis annab true tulemust
else 
    direktiiv_2 - täidetakse kui loogiline avaldis annab false tulemust
```
* Tingimusdirektiiv algab sõnaga if, millele järgneb ümarsulgudes loogiline avaldis (avaldis, mille väärtus saab olla kas tõene (`true`) või väär (`false`)) ja sellele omakorda direktiiv, mis täidetakse siis, kui loogiline avaldis on tõene (`true`). 

* Sõnale else aga järgneb direktiiv, mis täidetakse siis, kui loogiline avaldis on väär (`false`). Ühe direktiivi rollis võib olla ka plokk (programmi lõik)

* Tingimusdirektiivi else osa võib ka üldse puududa
```
if (loogiline avaldis) 
    direktiiv_1 - täidetakse siis, kui loogiline avaldis annab true
```
### Näidised
#### Absoluutväärtuse leidmine
<img src="http://anna.ikt.khk.ee/aa_ita19/14.01/absoluutvaartus.png" width="500" alt="absoluutvaartus.png">

#### Kehamassiindeksi väärtuse järgi inimese tervise hindamine
<img src="http://anna.ikt.khk.ee/aa_ita19/14.01/kmi.png" width="500" alt="absoluutvaartus.png">

## Teoreetiline materjall
[Tingimuslause](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/tingimuslause/)

## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks4`
* Salvesta antud kaustas kõik antud praktikumi programmid

### Ülesanne 1
Kirjutada programm, mis arvutab kahe reaalarvu jagatise. Programm peab väljastama mõlema arvu ja jagatise väärtused. Juhul, kui antud operatsioon ei ole võimalik sooritada, tuleb väljastada seletav teade (mis juhtum see on?).

Salvesta fail nimega `mata2.fprg`

### Ülesanne 2
Kirjutada programm, mis arvutab rõnga pindala. Programm peab kontrollima, kas rõnga raadius on suurem, kui rõnga augu raadius. Vastusel juhul tuleb väljastada seletav teade.

Salvesta fail nimega `mata3.fprg`

### Ülesanne 3
Kirjutada programm, mis teisendab minutid ja sekundid sekunditeks. Minutite ja sekundite defineerimiseks kasutada real tüüpi, väärtused on komaga arvud, kus täisosa on minutite arv ja osa, mis on kirjutatud peale koma on sekundite arv (Näiteks 1.45 on 1 minut 45 sekundit). 

Programm peab kontrollima omistatud väärtuste õigsust (Näiteks väärtus ei saa olla võrdne 2.90, kuna sekundite maksimaalne väärtus on 60, kuid väärtus 2.40 on võimalik, see vastab 2 minutile ja 40 sekundile)

Salvesta fail nimega `aeg.fprg`

### Ülesanne 4
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 5
Kopeeri `AA` kataloogs oleva `praks4` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
# 10.01
## Tunni teemad
* Andmetüübid ja väärtused
    * String (Sõne, Tekst) - `"Tere Hommikust!"`, `"Mart"` jne
    * Integer (Täisarv) - `1` ,  `2` , `-56` jne
    * Real (Komaga arv) - `2.5` , `-7.8` jne
    * Boolean (tõeväärtus) - `true`, `false`
* Muutujad
    * defineerimine - `andmetüüp muutujanimi`
        * näiteks `String kasutaja`
    * omistamine - väärtuse salvestamine - `muutujanimi = väärtus`
        * näiteks `kasutaja = "Mart"`
    * väljastamine
        * `output(kasutaja)`
* Operaatorid
    * Matemaatilised operaatorid
        * liitmine `+`
        * lahutamine `-`
        * korritamine `*`
        * jagamine `/`
        * jäägi leidmine `%`
        * asmesse panek `^`
* Avaldised
    * `operand1 operaator operand2`
    * näiteks 
        * omistamise avaldis `nimi = "Karli"`
        * liitmise avaldis `1 + 2` või `a + 3` või `a + b`
        * lahutamise avaldis `a - 2` või `a - c`
        * korrutamise avaldis `a * 2` või `b * d`
        * jagamise avaldis `s / 5` või `s / f`
        * jäägi leidmise avaldis `h % 2` või `4 % 2`
* Väljundi moodustamine
    * väljastada võib lihtsalt teksti, näiteks `"Tere tulemast, Mart!"`
    * väljastamisel võib kasutada ka ette defineeritud ja väärtustatud muutujad
        * näiteks `output("Tere tulemast, " & kasutajanimi)` - selleha me ühendame testiline väljund koos väärtusega, mis salvestasime muutujas
## Teoreetiline materjall
[Andmetüübid](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/andmetuubid/)

[Muutujad](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/muutujad/)
## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks2`
* Salvesta antud kaustas kõik antud praktikumi programmid
### Ülesanne 1
Defineeri kõikidega teatud andmetüüpidega muutujad ja omistada vastavad väärtused. Väljastada vastavate muutujate väärtused koos kirjeldusega, mis on antud tüübi karakteristik. Näiteks, `defineeritud täisarvu tüüpi muutuja nimega i, ja temale omistatud väärtus 2`. 

Salvesta fail nimega `andmetyybid.fprg`
### Ülesanne 2
1. Defineerida vähemalt 5 `Integer` tüüpi muutujat, näiteks nimedega `a`, `b`, `c`, `d`, `e`, `f` ja omistada muutujatele erinevad väärtused, kuid `a = 2147483647`.
2. Siis teosta kõikide muutujatega liitmise, lahutamise, korrutamise ja jagamise operatsioonid.
3. Kontrollige ka see, et mis saab siis, kui muutuja a väärtusele liita 1.
4. Leida jagatised 9/3, 7/4, -3/2, 3/(-2), -7/(-3).
5. Proovida leida jääki nii positiivsetest kui ka negatiivsetest arvudest.
* Tulemused väljastada nii:
`output("Arvude " & b & " ja " & c & " summa on " & (b + c));
    * Mis juhtub, kui avaldises (b + c) sulud ära jätta?

Salvesta fail nimega `mata1.fprg`
### Ülesanne 3
Inimeste transportimisks ühest kohast teise soovitatakse tellida teatav arv ühesuguseid busse. Antud on inimeste arv ja kohtades arv ühes bussis. Kõik bussid peavad saama täiesti täis. Ülejäänud inimesed jäävad maha. Koostage programm selle ülesanne lahendamiseks.

Sisu alguseks võtke kasutusele muutujad inimese arvu jaoks ja ühe bussi kohtade arvu jaoks ning andke nendele muutujale algväärtused.

Programm peab väljastama:
inimeste arvu
kohtade aru ühes bussis
busside arvu
bussidesse mahtunud inimeste arvu
mahajäänud inimeste arvu

Ülesanne lahendamiseks kirjeldage vajalikud muutujad ning pange kirja kõik avaldised, mille järgi tehakse arvutusi (jäägi leidmiseks kasutada `%` operaatori). 

Väljatrükk peab koosnema täislauseteks.

Salvesta fail `buss.fprg`
### Ülesanne 4
Küpsisetordi tegemisel laotakse terved ruudukujulised küpsised ristkülikukujulisele kandikule. Kandikule mahub ühes kihis `kandikuPikkus * kandikuLaius` küpsist. Laotakse `tordiPaksus` kihti. Ühes küpsisepakis on `küpsistPakis` küpsist. Püstitage ülesanne küpsisetordi tegemise kohta ja lahendage see. Programm peab väljastama ülesande püstituse ja kõik algväärtuseid ja tulemusi.

Salvesta fail `tort.fprg`
### Ülesanne 5
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 6
Kopeeri `AA` kataloogs oleva `praks2` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
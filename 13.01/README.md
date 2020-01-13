# 13.01
## Tunni teemad
* Tõeväärtused
    * `Boolean` tüüpi väärtused
    * `true` - tõene
    * `false` - väär

Loogika operaatorite väärtuste tabel:
* `a` - tõeväärtus
* `b` - tõeväärtus
* `c = a && b` - and - JA 
* `d = a || b` - or - VÕI
* `e = !a` - not - EITUS

|a|b|c|d|e|
|:---:|:---:|:---:| :---:|:---:|
`false`|`false`|`false`|`false`|`true`
`true`|`false`|`true`|`false`|`false`
`false`|`true`|`true`|`false`|`true`
`true`|`true`|`true`|`true`|`false`

## Teoreetiline materjall
[Andmetüübid](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/andmetuubid/)

[Muutujad](https://web.htk.tlu.ee/digitaru/programmeerimine/chapter/muutujad/)
## Ülesanded lahendamiseks
### Ettevalmistus
* <b>Kui ei ole veel tehtud</b>, siis loo `K:` kettal kataloog nimega `AA`
* Loo iga praktikumi jaoks eraldi kataloog nimega `praksNR`, kus `NR`on vastava praktikumi number - tänaseks siis `praks3`
* Salvesta antud kaustas kõik antud praktikumi programmid
## Kordamiseks ülesanded
### Ülesanne 1
On antud ringi ümbermõõt (reaalarv). Leida selle ringjoonega piiratud ala pindala. 

Salvesta fail nimega `ringi_pindala.fprg`
### Ülesanne 2
Antud on kolmnurga küljed a, b, c (reaalarvud). Leida pindala [Heroni valemi](https://et.wikipedia.org/wiki/Heroni_valem) järgi. Ruutjuure arvutamiseks kasutame funktsiooni `Sqrt(väärtus)`, mis arvutab väärtuse ruutjuure. Väärtus on võimalik tekitada dünaamiliselt - ehk valemi abil.

Salvesta fail nimega `kolmnurk_heron.fprg`
### Ülesanne 3
Leida võrdkülgse kolmnurga pindala, kui on antud ümbermõõt p (reaalarv).

Salvesta fail `kolmnurk_vordkylgne.fprg`
### Ülesanne 4 
Antud on [täisnurkse](https://et.wikipedia.org/wiki/T%C3%A4isnurkne_kolmnurk) kolmnurga kaatetid (reaalarvud). Leida hüpotenuus ja pindala.

Salvesta fail `kolmnurk_taisnurkne.fprg`
## Tõeväärtused
Kontrollida kõikide a, b, c, d väärtuste kombinatsioonide korral, et antud tingimus kehtib: `a && b || c && d` on sama nagu `(a && b) || (c && d)`. Väljastada iga väärtuste kombinatsiooni korral nii `a`, `b`, `c`, `d` väärtused kui ka vahearvutuste tulemused ning tulemuse:
Näiteks osa väljastamisest:
```
a = true
b = true
c = true
d = true
---------------------------------
a && b = true
a && b || c = true
a && b || c && d = true
---------------------------------
(a && b) = true
(c && d) = true
(a && b) || (c && d) = true
---------------------------------
Kehtib!
```
Spikker: Kõikide väärtuste kombinatsioonide leidmiseks tuleb leida, millega on võrdne 2<sup>muutujate_arv</sup>. Näiteks antud juhul kasutame 4 muutujat, seega väärtuste kombinatsioonide arv on 2<sup>4</sup>=16. Kõikide väärtuste leidmiseks parem koostada järgmise tabeli: (t - tõene (true), v - väär (false) )

|a|b|c|d|
|:---:| :---:|:---:|:---:|
`t`|`t`|`t`|`t`
`t`|`t`|`t`|`v`
`t`|`t`|`v`|`t`
`t`|`t`|`v`|`v`
`t`|`v`|`t`|`t`
`t`|`v`|`t`|`v`
`t`|`v`|`v`|`t`
`t`|`v`|`v`|`v`
`v`|`t`|`t`|`t`
`v`|`t`|`t`|`v`
`v`|`t`|`v`|`t`
`v`|`t`|`v`|`v`
`v`|`v`|`t`|`t`
`v`|`v`|`t`|`v`
`v`|`v`|`v`|`t`
`v`|`v`|`v`|`v`

### Ülesanne 5
Varusta kõik oma programmid kommentaaridega:
* failinimi
* autor  - Ees ja Perenimi
* programmi loomise kuupäev
* programmi versioon (0.1 - algversioon, 0.2 - parandused pärast salvestamist jne)
### Ülesanne 6
Kopeeri `AA` kataloogs oleva `praks3` kataloog GoogleDrive-i ja <b>kui ei ole veel seda teinud, siis</b> jaga [anna.karutina@khk.ee]("mailto:anna.karutina@khk.ee") vaatamisõigustega.
# Úmrtia v ČR

Vzťah medzi pozitívne testovanými a úmrtiami s covid-19.

Je to dávnejšie, čo Janek Ledecký zverejnil [video](https://tn.nova.cz/clanek/prestante-nas-strasit-znamy-zpevak-se-rozohnil-kvuli-koronaviru.html) podľa ktoreho: "...počet úmrtí nevykazuje žádnej růst..."

A na tento "nevykazaný" nárast by som sa rád pozrel.

# Data

Data som cerpal z [verejne dostupnych dat pre CR](https://onemocneni-aktualne.mzcr.cz/covid-19).

Len som mierne upravil formát, aby ich vzal môj MS Excel. Použil som dáta za od 1.7.2020 (čisto z lenivost = v úmrtiach boli diery = dny keď nikto neumrel a preto som to ručne opravil, aby to sedelo len späť od 1.7.2020).

# Graf 1 - "à la Ledecký"

![Graf 1](/files/graf1_big.png)

Je podobny tomu, čo prezentuje Ledecký. Nie je patrný žiadny nárast.

**Problém:** nárast nie je vidieť, lebo tie čísla úmrtí su rádovo (100x menšie)

# Graf 2

Problém z grafu 1 sa dá ľahko vysvetliť, tým, že sa zmení mierka pre úmrtia. Excel rozmedzia nastavil automaticky:
- 0 - 5000 pre pozitívne testovaných
- 0 - 35 pre úmrtia

![Graf 2](/files/graf2_big.png)

# Graf 3

Graf 2 je moc detailný a obávam sa toho, ze ta dôležitá informácia sa v tých detailoch stratí a bude nabádať na nevalídny argument "skače to hore-dole".

Je to niečo na spôsob "pre stromy nie je vidieť les"...

Preto som sa rozhodol použiť 4-dňový kĺzavý priemer, aby sa tie krivky !vyhladili". Prečo 4-dňový? Jednoducho preto, aby boli 2 víkendové dni (keď sa testuje menej) vykompenzované.

![Graf 3](/files/graf3_big.png)

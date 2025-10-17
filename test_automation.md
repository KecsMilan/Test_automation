# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

## A tesztelés alapjai:

#### Mi a tesztelés célja? Mi nem az?

<img src="https://startupsmagazine.co.uk/sites/default/files/2022-02/AdobeStock_309443011ed.png" height="100px" width="250px">

    ✅ célja	=> hibák felderítése (bug, visual), és utána dokumentálása
    ❌ nem célja => tökéletes-re törekedni (hiba mentes), mert mindig lesznek hibák

#### Mi a kapcsolat a tesztelés és a hibamegelőzés között?
    A hiba megelőzés folyamata a tesztelés, ahol felfedezett hibákat javítjuk (megelőzzük)

#### Miért fontos, hogy a tesztelők függetlenek legyenek a fejlesztőktől?
    Objektív vizsgálat
    Kritikus hang

#### Mi a veszélye annak, ha a fejlesztő maga teszteli a saját kódját?
    Elfogultság (nem reális)
    Nem felhasználó barát megközelítés (javaslatok hiánya)
    Nem feltétlen tud mások fejével gondolkodni (triviális hibák)

#### Mik a tesztelési alapelvek?
#####    1. Teszt:
     Kimerítő tesztelés nem lehetséges (nincs erőforrás végtelen teszt eset felállítására és kipróbálására)

#####    2. Hibafürt:
     A tesztelés folyamán az egész software-t kisebb részekre (nagyobb % hiba terület) bontjuk

#####    3. Növényvédő szer-paradoxon:
     Amikor a tesztelés során, ugyan azokat végezzük el, nem kísérletezünk újjal ("új kártevők" = new bugs ? "feature")

#####    4. Bizonyítja vannak hibák:
     Azt jelenti, hogy van még mit javítani, sosem képes teljes mértékben hiba mentes lenni

#####    5. Hiba hiánya:
     Új teszt esetek kigondolását jelenti, ha nem találunk hibát, találnunk kell!

#####    6. Korai teszt:
     A legkritikusabb időszak a software megjelenése előtt a "béta" = teszt fázis, de már jóval előtte is tesztelni kell folyamatosan, ahogy szerkesztjük a kódot.
    
#####    7. Kontextus:
     Nem mindegy, hogy éppen milyen software-t milyen környezetben tesztelünk pl. windows app (Windowson és NEM Linuxon vagy MacOS-en)

#### Mit jelent az „alapvető tesztelési elv”, hogy „a kimerítő tesztelés lehetetlen”?
    Nincs erőforrás végtelen teszt eset felállítására és kipróbálására, illetve a kreatívitás egy idő után csökken.

#### Mit jelent az „alapvető tesztelési elv”, hogy „a hibák halmozódnak”?
    Ahogy szerkesztjük a kódot, újabb hibákat szülhet.

#### Mit jelent az „alapvető tesztelési elv”, hogy „a tesztelés a kontextustól függ”?
        Nem mindegy, hogy éppen milyen software-t milyen környezetben tesztelünk pl. windows app (Windowson és NEM Linuxon vagy MacOS-en)
		megfelelő működés elérése => megfelelő környezet.

## 2. Tesztelés a szoftverfejlesztés életciklusán át
#### Mik a tesztszintek, és mi a különbség köztük?
#####    1. Egységtesztelés 
     => egy adott rész (új funkció) tesztelése

#####    2. Integrációs tesztelés
     => hogyan kommunikál a kód egyes részei egymással

#####    3. Rendszer
     => különböző operációs rendszereken, hogyan fut, illetve összességében, hogyan megy 

#####    4.Fogadás
     => megfelel-e a megrendelő elvárásainak

#### Miért nem érdemes mindig ugyanazokat a teszteseteket futtatni (regressziós torzítás)?
    Mert nem figyelünk fel új hibákra, amik keletkeznek a régi hiba kijavítása után

#### Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
    Egy adott rész (új funkció) tesztelése, fejlesztő által, fejlesztő feladata, illetve bevont tesztelő (megadott utasítás alapján).

#### Mi a különbség a verifikáció és a validáció között?
#####    Verifikáció
     => minőség ellenőrzés
#####    Validáció 
     => megfelel-e a követelménynek ellenőrzés

#### Mik a tesztelési típusok, és mi a különbség köztük?
#####    [Funkcionális tesztelés]:
			-Egységtesztelés
			-Integrációs
			-Rendszer
			-Fogadás

#####	[Nem-funkcionális]:
			-teljesítmény
			-terhelés

#####	[Biztonsági]:
			-adatvédelem
			-sérülékenységek

#####	[Használhatósági]:
			-felhasználó barát
			-irodai környezet barát
			-infrastruktúra barát (céges környezet)

#####	[Automatizált tesztelés]:
			-meglévő teszt esetek automatizált tesztelése

#### Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
#####    Fehér doboz
     => a forráskód ismerete (statikus)
#####    Fekete doboz
     => anélkül (dinamikus)
#####    Szürke doboz
    => a kettő kombinálva ( statikus és dinamikus tesztelés )

#### Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
#####    [felhasználói]:
        -megfelel-e a követelményeknek

#####    [rendszerteszt]:
        -bírja a teljesítményt ( terhelés alatt )
        -biztonságos-e

#### Mi a különbség a statikus és dinamikus tesztelés között?
#####    Statikus
     => a forráskód ismerete (Fehér doboz)
#####    Dinamikus
     => a forráskód ismerete nélkül (Fekete doboz)

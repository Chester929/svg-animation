Časování
========
__"presentation time"__: označuje bod v čase vzhledem k začátku části dokumentu
__"fill"__: určuje, jestli se animace po skončení zastaví na poslední hodnotě, nebo jestli zmizí
__"syncbase"__: označuje animaci pro synchronizaci (animace může začít současně s koncem nebo začátkem jiné animace)
__keyTimes__: seznam hodnot týkající se daného okamžiku animace - ovlivňují průběh animace (hodnoty od 0 do 1 určující časový bod)
__keySplines__: souvisí s keyTimes; čtveřice hodnot (0 - 1) reprezentujících umístění kontrolních bodů křivky, která určuje tempo animace

přechod (calcMode)
--------
__diskrétní__: skočí se z jedné hodnoty na druhou bez přechodu
__lineární__: přechod je založen na funkci vzniklé lineární interpolací
__"paced"__: přechod stálé rychlosti
__křivkou__: animace je definována Bézierovou křivkou (viz keyTimes a keySplines)

Aditivita
========
__"additive"__: animace nenahrazuje předchozí hodnoty atributů, ale staví na nich
__"accumulate"__: při opakování neprobíhá animace od začátku, ale navazuje na předchozí výsledek (výsledná hodnota se přičte k počáteční hodnotě)

Pohyb (animateMotion)
=====================
__dráha__: křivka, po které se pohybuje animovaný objekt
__keyPoints__: seznam floatů mezi 0 a 1, určuje délku pohybu po určené dráze podle časů v keyTimes; seznam musí mít stejnou délku jako keyTimes

Transformace (animateTransform)
===============================
__viewport__: výřez, v kterém se nachází SVG obrázek; v našem případě stránka
__původní soustava souřadnic__: soustava souřadnic, jejíž počátek je v počátku viewportu
__nová soustava souřadnic__: soustava souřadnic vzniklá transformací původní soustavy souřadnic
__trasformační matice__: matice ve tvaru
a c e
b d f
0 0 1
, kterou když přenásobíme souřadnicemi nové soustavy souřadnic [x y 1]T zprava, tak získáme souřadnice původní soustavy souřadnic

__type = "translate | scale | rotate | skewX | skewY"__: Označuje druh transformácie, ktorá sa dá svojími hodnotami meniť v priebehu. Pokiaľ atribút nie je zadáný, defaultne sa používa hodnota 'translate'.

__‘from’__, __‘by’__ a __‘to’__ sú atribúty vyjadrené pomocou rovnakej syntaxie, ktorá je k dispozícii pre daný typ transformácie::

Pre typ = "translate", je každá jednotlivá hodnota vyjadrená ako '<tx> [, <ty>]'. 
Pre typ = "scale", je každá jednotlivá hodnota vyjadrená ako '<sx> [, <sy>]'. 
Pre typ = "rotate", je každá jednotlivá hodnota vyjadrená ako '<rotate-angle> [<cx> <cy>]'. 
Pre typ = "skewX" a pre typ = "skewY", je každá jednotlivá hodnota vyjadrená ako '<skew-angle>'.

Atribút __additive__ nám určuje chovanie animácie.

__additive="replace"__: Nahradí povodný frame.
__additive="sum"__: Doplní, alebo usekne povodný frame.


Změna barvy (animateColor)
==========================

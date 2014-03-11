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

Změna barvy (animateColor)
==========================

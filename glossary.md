Časování
========
přechod (calcMode)
--------
__diskrétní__: skočí se z jedné hodnoty na druhou bez přechodu \\ 
__lineární__: přechod je založen na funkci vzniklé lineární interpolací
__"paced"__: přechod stálé rychlosti
__křivkou__: animace je definována Bézierovou křivkou (viz keyTimes a keySplines)
__"keyTimes"__: seznam hodnot ovlivňující tempo animace (hodnoty od 0 do 1 určující časový bod v průběhu animace)
__"keySplines"__: souvisí s keyTimes; čtveřice hodnot (0 - 1) reprezentujících umístění kontrolních bodů křivky, která určuje tempo animace

Pohyb (animateMotion)
=====================
__keyPoints__: seznam floatů mezi 0 a 1, určuje délku pohybu po určené dráze podle časů v keyTimes; seznam musí mít stejnou délku jako keyTimes

Transformace (animateTransform)
===============================

Změna barvy (animateColor)
==========================

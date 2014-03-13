Časování
========
* na rozdíl od SMIL a tudíž i SVG animací, flash animace používají keyframes jakožto hlavní body animace, zobrazené na časové ose  
* délka animace je tedy určena počtem framů  
* v každém framu můžeme vidět, jak bude stav animace v tomto bodě vypadat a případně upravit změnou na keyframe a nastavením nějaké hodnoty  
* tempo animace je možné nastavit pomocí křivky pro náběh/doběh  

Pohyb (Motion tween)
=====================
* pohyb se vytváří pomocí křivky, která vznikne volbou "vytvořit doplnění pohybu" a přemístěním daného tvaru na požadované místo
* pohyb lze také vytvořit pravým klikem mezi dva klíčové framy a zvolením možnosti pro doplnění pohybu
* křivka se dá pomocí nástrojů na výběr upravovat - rotovat, měnit velikost a klíčovým snímkem se přidá uzel  

Transformace (Shape tween)
===============================
* pomocí změny tvaru (velikost, rotace,...) objektu v daném keyframu dojde k vytvoření přechodu tvaru  
* je možné vytvořit animaci interpolace dvou objektů - ve dvou framech na časové ose se vytvoří různé objekty a v nějakém framu mezi nimi se zvolí možnost doplnit tvar  

Změna barvy (Color tween)
==========================
* v jednotlivých keyframech je možné nastavit ve vlastnostech objektu barvu (odstín, alfa, jas), čímž vložíme do animace přechod barvy  

Skripty
==========================
* skripty se dají vytvářet v jednotlivých framech animace, ve kterých jsou při běhu animace spuštěny

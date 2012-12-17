czech.lbx
=========

Toto je česká podpora pro biblatex. Vychází ze souboru `czech.lbx`, který je distribuován s balíčkem biblatex-iso690 [1]. 
Tento starší soubor byl určený hlavně pro potřeby biblatex-iso690 a zůstal v provizorním stavu. 
Termíny které tento styl nevyužíval zůstaly nepřeložené, byly přidány některé nestandardní termíny, 
text byl kódovaný v kódování utf-8, což přinášelo problémy v dokumentech psaných v jiných kódováních. 

Protože jsem v poslední době zaznamenal zvýšený zájem o českou podporu pro biblatex, rozhodl jsem se napravit 
výše zmíněné nedostatky a vytvořil nový lokalizační soubor. Ten vychází ze současných lokalizačních řetězců pro biblatex
verze 2.4 a měl by obsahovat překlad všech termínů. 

Upozornění
----------

Zatím se jedná o ranou verzi, která potřebuje důkladné testování, než bude nabídnuta do oficiální distribuce biblatexu. 
Pokud najdete jakoukoli chybu, buď opravte přímo její výskyt v souboru `czech-utf-source.lbx` a proveďte pull request,
nebo kontaktujte autora [2]

Použití
-------

Zdrojové texty lokalizace jsou obsažené v souboru `czech-utf-source.lbx`, kde jsou termíny zapisované v kódování
utf-8. Z důvodů kompatibility je třeba tento soubor zkonvertovat do kódování ASCII s využitím TeXových sekvencí pro 
diakritiku. Pro tento účel je určený skript uni2tex, který lze spoustit tímto způsobem:

    python uni2tex czech-utf-source.lbx > czech.lbx

Licence
-------

GNU/GPL 3 


[1] https://github.com/michal-h21/biblatex-iso690

[2] michal.h21 zavinac gmail tecka com

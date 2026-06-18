# Short Tandem Repeats Detection

Il notebook applica un filtro _Sliding Window Quality_ per effettuare il trimming del read al 3’ usando una finestra scorrevole, di dimensione configurabile, troncando opportunamente il read non appena la qualità 
media all’interno della finestra scende al di sotto di una certa soglia. 

All’interno dei reads rimasti alla fine del precedente filtraggio, vengono riconosciuti gli Short Tandem Repeats (STRs) di lunghezza 1, 2 e 3. 
Uno Short Tandem Repeat è una sottostringa massimale in cui un certo motivo (lungo qualche base) si ripete un certo numero di volte.

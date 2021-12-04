### Zadanie 1
Foldery dostępne dla mnie mają nadane uprawnienia g+x, pliki g+r. Do stworzenia pliku w katalogu potrzebuje uprawnień g+w i g+x. "Podrzucony" plik mogę usunąć gdy jestem właścicielem katalogu nadrzędnego - pojawia się komunikat o nadpisaniu uprawnień.
### Zadanie 2
Komendę ```cd``` możemy wykonać na katalogach których mamy nadane prawa wejścia. ```chmod``` wtedy kiedy jesteśmy właścicielami katalogu. Jeżeli do katalogu nadrzędnego nie mamy prawa wstępu ale mamy do katalogu podrzędnego to nie mamy możliwości wejścia do podrzędnego
### Zadanie 3
Operator ```>```  usuwa stare dane, a ```>>``` dopisuje je na strumień wyjściowy.
```tail -f plik```  Otwiera plik i wypisuje na bierząco dopisane linijki tekstu. 

### Zadanie 4
Po utworzeniu i nadaniu praw odczytu dla pliku ```strona.html``` i prawa wejścia dla wszystkich dla katalogów ```public_html``` oraz katalogu domowego - Apache zwraca błąd 404. Podejżewam że może to być związane z błędną konfiguracją Apache, gdyż nie ma nawet dostępu do pluku html na którą jest ustawione przekierowanie z adresu domowego. Wszystkie katalogi nadrzędne mają przyporządkowane prawa wejścia i odczytu
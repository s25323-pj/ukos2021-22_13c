### Zadanie 1
Ścieżka względna
```
$ cd ../../../kot/ma/ale
```
Ścieżka bezwzględna
```
& cd /tmp/ukos/kot/ma/ale
```
### Zadanie 2
```
mkdir -p ../../../kot/ma/ale/jan/kowalski
```
### Zadanie 3
```
mv ../../../kot/ma/ale ../../i/
```

### Zadanie 4
Pobieramy PID procesu który chcemy zamknąć 
```
$ ps -a
```
I zabijamy go komendą kill:
```
$ kill -9 [PID procesu]
```
### Zadanie 5
```
$ ls -p | grep -v / | grep -e ^al
```
### Zadanie 6
```
$ chmod a+x,g+r,u+rwx ala
$ chmod 751 ala
```
### Zadanie 7
```
$ ls -p | grep -v / >> lista_plikow.txt
```

### Zadanie 8
1. Brak miejsca na dysku
2. Brak uprawnień

### Zadanie 9
Używając klawisza tab.

### Zadanie 10
1. Używając ampersandu
```
$ nano &
```
2. Uruchomić program i użyć skrótu ctrl + z
```
$ nano ^Z
```
 
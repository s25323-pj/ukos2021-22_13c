### Zadanie 1
```
60386:~ rafal$ ps
PID TTY TIME CMD
56669 ttys005  0:00.08 -bash
```
```
60386:~ rafal$ ps -a
PID TTY TIME CMD
56668 ttys005  0:00.31 login -pf rafal
56669 ttys005  0:00.08 -bash
60480 ttys005  0:00.00 ps -a
```
```
60386:~ rafal$ ps x
PID TT  STAT  TIME COMMAND
439 ??  S  7:27.17 /usr/sbin/distnoted agent
443 ??  S  7:33.52 /usr/sbin/cfprefsd agent
444 ??  S 10:13.82 /usr/libexec/UserEventAgent (Aqua)
...
```
```
60386:~ rafal$ ps aux
USER PID  %CPU %MEM  VSZ  RSS TT  STAT STARTED  TIME COMMAND
rafal  36720 6,6  3,9 17415032 1304388 ??  S  czw10 141:22.22 com.docker.hyperkit -A -u -F vms/0/hyperkit.pid -c 8 -m 12288M -s 0:0,hostbridge -s 31,lpc -s 1:0,virtio-vpnkit,path=vpnkit.eth
_windowserver  147 3,6  0,5 12636648 156216 ??  Ss  4lis21 2814:29.46 /System/Library/PrivateFrameworks/SkyLight.framework/Resources/WindowServer -daemon
...
```
Znak ? pod kolumną TT oznacza że powłoka w której został uruchomiony proces została zamknięta.
```
$ ps aux
```
```
$ ps aux -U 
```

### Zadanie 2

```
$ ps -a
```
```
$ kill 60848
```
z SiGKILL
```
$ kill -9 60848
```
```
$ killall shell
No matching processes belonging to you were found
```
```kill``` działa tylko wtedy gdy mamy uprawnienia do zabicia konkretnego procesu.

### Zadanie 3
```
$ cat > wynik1.txt
witaj^C
$ cat wynik1.txt
```
Został stworzony pusty plik, dane nie zapisały się do niego

```
$ cat > wynik2.txt
witaj^D
$ cat wynik2.txt
witaj$
```
Został stworzony plik, dane zostały zapisane
### Zadanie 4
```
$ gimp &
& gedit &
$ geany &
$
$ jobs
[1]   7893 Running gimp &
[2]   7894 Running gedit &
[3]   7895 Running geany &
...
$ fg 3
```
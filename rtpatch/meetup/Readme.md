Plan :

1 - Pres' du patch preempt-rt
A quel besoin ça répond ? déterminisme dans les latences, RT soft
Dans quel cas on l'utilise ? besoin de déterminisme + necessité d'avoir un linux
2 - Quel impact ?
Outils de monitoring système usuels:
htop - métriques load-avg, %age CPU ( user - kernel - IO ), nb process/threads/kthreads
iostat - Vitesse IO
/proc/interrupts - NB interrupts
iotop - 
sar ?
vmstat
/proc/watever
pidstat -w 10 1
schedtop ?





# Slides PreemptRT


# Compilation du PDF
make mr\_proper all

Nécessite texlive et imagemagick

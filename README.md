README.md

En un principio la idea es poder usar estos scripts con https://github.com/liamsgotgenes/xfce4-theme-switcher aunque se puede usar para lanzar cualquier orden

Dependencias: 
jq 
https://archlinux.org/packages/community/x86_64/jq/
https://man.archlinux.org/man/community/jq/jq.1.en

crontab
https://wiki.archlinux.org/title/Cron
https://archlinux.org/packages/?name=cronie


y de las siguientes apis:
https://api.sunrise-sunset.org
https://ip-api.com/

Basta con programar que se ejecuten al inicio de sesión

EditCron llama a DayOrNight por lo que o se espefica la ruta a mano o se guarda en bin ejm /usr/local/bin

BUGS
Deberia corregir al script para no borrar el resto de tareas programadas
YEP aun tengo que ampliar el readme y depurar código

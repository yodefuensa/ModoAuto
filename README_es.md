Dependencias: 
jq 
https://archlinux.org/packages/community/x86_64/jq/
https://man.archlinux.org/man/community/jq/jq.1.en

cron
https://wiki.archlinux.org/title/Cron
https://archlinux.org/packages/?name=cronie

script:
https://github.com/liamsgotgenes/xfce4-theme-switcher

y de las siguientes apis:
https://api.sunrise-sunset.org
https://ip-api.com/

Funcionamiento. Son 2 scripts:
DayOrNight ejecuta un script u otro en base a si es de día o de noche. En este caso se ejecuta usamos "xfce4-theme-switcher" para cargar 2 temas que tenemos que tener previamente creados. Para que funciones DayOrNight debes haber creado previamente las configuraciones "day" y "night" tambien puedes crear tus temas propias configuracións o sustiuir la lineas 38 y 41 por las que consideres

EditCron: Crea un fichero cron la shell y varibles del usaurio y programa la ejecución de DayOrnight a la hora del anochecer


Inslación

1.  Instala xfce4-theme-switcher
2.  Configura los temas day y night
3.  Instala cron en tu distro y habilita el servicio
4.  Copia los scripts DayOrnigh Y EditCron a /usr/local/bin
5.  Establece que los scripts se ejecuten al iniciar sesión 





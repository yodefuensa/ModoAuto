
# Cambio de tema automatico XFCE4
Este proyecto consta de dos scripts que permiten cambiar automáticamente el tema de XFCE4 en función de si es de día o de noche.

## Dependencias
- jq https://archlinux.org/packages/community/x86_64/jq/
- cron https://wiki.archlinux.org/title/Cron
- xfce4-theme-switcher https://github.com/liamsgotgenes/xfce4-theme-switcher

Además, se utilizan las siguientes APIs:
- Sunrise-Sunset API https://api.sunrise-sunset.org
- IP-API https://ip-api.com/

## Funcionamiento
El script `DayOrNight` decide si ejecutar un script u otro en función de si es de día o de noche. En este caso, se utiliza "xfce4-theme-switcher" para cargar dos temas que debes tener previamente creados. Para que funcione `DayOrNight`, debes haber creado previamente las configuraciones "day" y "night". También puedes crear tus propios temas o sustituir las líneas 38 y 41 por las que consideres.
`EditCron` crea un fichero cron con la shell y las variables del usuario, y programa la ejecución de `DayOrNight` a la hora del anochecer.

## Instalación
1. Instala `xfce4-theme-switcher`.
2. Configura los temas `day` y `night`.
3. Instala `cron` en tu distro y habilita el servicio.
4. Copia los scripts `DayOrNight` y `EditCron` a `/usr/local/bin`.
5. Establece que los scripts se ejecuten al iniciar sesión.



Dependencies:

jq
https://archlinux.org/packages/community/x86_64/jq/
https://man.archlinux.org/man/community/jq/jq.1.en

cron
https://wiki.archlinux.org/title/Cron
https://archlinux.org/packages/?name=cronie

script:
https://github.com/liamsgotgenes/xfce4-theme-switcher

and the following APIs:
https://api.sunrise-sunset.org
https://ip-api.com/

Operation: There are 2 scripts:

DayOrNight runs one script or another depending on whether it is day or night. In this case, it is executed using "xfce4-theme-switcher" to load 2 themes that we must have previously created. For DayOrNight to work, you must have previously created the "day" and "night" configurations. You can also create your own configurations or replace lines 38 and 41 with whichever you deem appropriate.

EditCron: Creates a cron file in the shell and user variables, and schedules the execution of DayOrNight at nightfall.

Installation:

    Install xfce4-theme-switcher.
    Configure the "day" and "night" themes.
    Install cron on your distribution and enable the service.
    Copy the DayOrNight and EditCron scripts to /usr/local/bin.
    Set the scripts to run at login.

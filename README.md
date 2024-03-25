# automatic xfce4 theme switcher
This project consists of two scripts that allow automatically changing the XFCE4 theme based on whether it's daytime or nighttime.

# Depndencies
    jq https://archlinux.org/packages/community/x86_64/jq/
    cron https://wiki.archlinux.org/title/Cron
    xfce4-theme-switcher https://github.com/liamsgotgenes/xfce4-theme-switcher

Additionally, the following APIs are used:
    Sunrise-Sunset API https://api.sunrise-sunset.org
    IP-API https://ip-api.com/

## Operation
The DayOrNight script decides whether to execute one script or another based on whether it's daytime or nighttime. In this case, "xfce4-theme-switcher" is used to load two themes that you must have previously created. For DayOrNight to work, you must have previously created the "day" and "night" configurations. You can also create your own themes or replace lines 38 and 41 with your preferences.
EditCron creates a cron file with the user's shell and variables, and schedules the execution of DayOrNight at sunset.

## Installation
1.   Install xfce4-theme-switcher.
2.   Configure the day and night themes.
3.   Install cron on your distro and enable the service.
4.   Copy the DayOrNight and EditCron scripts to /usr/local/bin.
5.   Set the scripts to run on login.
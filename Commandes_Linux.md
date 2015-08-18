Connaître :

+ La date et l'heure du système : ```date```

```
jb@ns378101:~$ date
mercredi 19 août 2015, 01:14:18 (UTC+0200)
```
+ Gestion des tâches planifiées :  ```crontab```

Pour lire la crontab de l'utilisateur courant ou celle de **root**

```
jb@ns378101:~$ crontab -l
no crontab for jb

jb@ns378101:~$ sudo crontab -u root -l
# Edit this file to introduce tasks to be run by cron.
#
# Each task to run has to be defined through a single line
# indicating with different fields when the task will be run
# and what command to run for the task
#
# To define the time you can provide concrete values for
# minute (m), hour (h), day of month (dom), month (mon),
# and day of week (dow) or use '*' in these fields (for 'any').#
# Notice that tasks will be started based on the cron's system
# daemon's notion of time and timezones.
#
# Output of the crontab jobs (including errors) is sent through
# email to the user the crontab file belongs to (unless redirected).
#
# For example, you can run a backup of all your user accounts
# at 5 a.m every week with:
# 0 5 * * 1 tar -zcf /var/backups/home.tgz /home/
#
# For more information see the manual pages of crontab(5) and cron(8)
#
# m h  dom mon dow   command

5 19 * * * cat /var/log/auth.log
```

Pour éditer la crontab de l'utilisateur courant ou celle de **root**

```
jb@ns378101:~$ sudo crontab -u root -l
```
  

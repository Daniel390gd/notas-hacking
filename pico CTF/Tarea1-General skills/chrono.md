
## Descripción 

How to automate tasks to run at intervals on linux servers?Use ssh to connect to this server:

```
Server: saturn.picoctf.net
Port: 64057
Username: picoplayer 
Password: ENAFb6zfzn
```
## Solución

- Nos conectamos al servidor con los datos que nos da la descripción.
- Usamos el comando cat /etc/ crontab para obtener la bandera.
![[02-chrono.png]]



```
picoCTF{Sch3DUL7NG_T45K3_L1NUX_1d781160}
```

## Referencias

- [How to Automate tasks in Linux using Crontab](https://www.linuxtechi.com/schedule-automate-tasks-linux-cron-jobs/)

## Descripción 

Play this short game to get familiar with terminal applications and some of the most important rules in scope for picoCTF.Connect to the program with netcat:`$ nc verbal-sleep.picoctf.net 63285`

### pista

When a choice is presented like [a/b/c], choose one, for example: `c` and then press Enter.
## Solución

- Con el comando nc nos conectamos a  nc verbal-sleep.picoctf.net 63285
- Nos ponemos a leer las indicaciones, cuando nos de a elegir opciones deberemos como dice la pista elegir una opción y dar enter.
- Repetir hasta obtener la bandera.
![[FANTASY-CTF_IMG1.png]]

![[FANTASY-CTF_IMG2.png]]

![[FANTASY-CTF_IMG3.png]]

```
picoCTF{m1113n1um_3d1710n_e41acbee}
```

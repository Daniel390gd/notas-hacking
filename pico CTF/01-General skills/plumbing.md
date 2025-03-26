## Descripción 

Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 7480`.

### pistas

- Remember the flag format is picoCTF{XXXX}
- What's a pipe? No not that kind of pipe... This [kind](http://www.linfo.org/pipes.html)

## Solución

1. Nos conectamos usando netcat a `jupiter.challenges.picoctf.org 7480`
2.  Redirigimos a un archivo llamado datos
3. usamos ls
4. Usamos cat y una pipeline" |"  con el comando grep para localizar la bandera


![[08-plumbing.png]]


```
picoCTF{digital_plumb3r_06e9d954}
```

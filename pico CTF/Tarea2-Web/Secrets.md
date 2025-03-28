
## Descripción 

We have several pages hidden. Can you find the one with the flag?The website is running [here](http://saturn.picoctf.net:65298/).
### pista

folders folders folders
## Solución

- Entramos a la pagina dada en la descipción.
- Observamos el html y vemos que hay una carpeta llamada secrets accedemos a ella en el navegador agregando en la url /secrets.
![[07-Secrets_IMG1.png]]
![[07-Secrets_IMG2.png]]
- Inspeccionando ahora hay una llamada hidden, repetimos lo hecho en el paso anterior.
![[07-Secrets_IMG3.png]]
![[07-Secrets_IMG4.png]]
- Volvemos a inspeccionar y encontramos ahora una carpeta llamada supersecret, repetimos lo hecho en los pasos anteriores.
![[07-Secrets_IMG5.png]]
- En esta ultima pagina inspeccionamos y obtenemos la bandera.
![[07-Secrets_IMG6.png]]





```
picoCTF{succ3ss_@h3n1c@10n_39849bcf}
```

## Referencias

- https://youtu.be/IfeMGQBq-XA?si=s2GpEWodGC6gMPHi
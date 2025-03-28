
## Descripción 

Can you get the flag?Go to this [website](http://saturn.picoctf.net:56099/) and see what you can discover.
### pista

Do you know how to modify cookies?
## Solución

- Entramos en la pagina dada por la descripción.
- Entramos como invitado.
![[05-Power-Cookie_IMG1.png]]
- Vemos que nos sale un mensaje sobre que no están disponibles las peticiones.
![[05-Power-Cookie_IMG2.png]]
- Usando el cookie editor cambiamos el valor de la cookie isAdmin a 1 y recargamos la pagina, obteniendo la bandera.
![[05-Power-Cookie_IMG3.png]]



```
picoCTF{gr4d3_A_c00k13_65fd1e1a}
```


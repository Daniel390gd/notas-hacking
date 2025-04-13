
## Descripción 

Help us test the form by submiting the username as `test` and password as `test!`The website running [here](http://saturn.picoctf.net:54339/).
### pista

any redirections?
## Solución


- Entramos en la pagina.
![[06-findme_IMG1.png]]
- Usamos las credenciales que nos dan.
![[06-findme_IMG2.png]]
- Observamos que sin importar que se nos redirige a la misma pagina.
- Usando burp suite y intentaremos interceptar.
![[06-findme_IMG3.png]]
- Obtenemos una parte de la bandera.
![[06-findme_IMG4.png]]
- Le damos en forward y obtenemos otra parte de la bandera.
![[06-findme_IMG5.png]]


```
picoCTF{proxies_all_the_way_be716d8e}
```

## Referencias

- https://youtu.be/2t3zK1dVMYA?si=ff-eVfviAaZ2J58S
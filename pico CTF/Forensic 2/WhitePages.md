
## Descripción 

I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/74274b96fe966126a1953c80762af80d/whitepages.txt) is all blank!

## Solución

- Con el comando wget descargamos el archivo .txt
![[02-WhitePages_IMG1.png]]
- Con el comando file vemos que el archivo es Unicode.
![[02-WhitePages_IMG2.png]]
- Usando el comando xxd vemos que se repite en hexadecimal e28083 que es un espacio en Unicode y aparte el espacio convencional (en hexadecimal 20).
![[02-WhitePages_IMG3.png]]
- Vamos a instalar pwntools.
![[02-WhitePages_IMG4.png]]
- Con la herramienta vamos a crear un archivo llamado exp.py donde vamos a convertir los espacios "e28083" a 0 y los normales "20" a 1 despues vamos a pasar todo a ascii y mostrarlo.
![[02-WhitePages_IMG5.png]]
- Guardamos y ejecutamos el archivo exp.py para obtener la bandera.
![[02-WhitePages_IMG6.png]]


```
picoCTF{not_all_spaces_are_created_equal_c54f27cd05c2189f8147cc6f5deb2e56}
```

## Referencias

- https://youtu.be/427HDV7tzow?si=m2aehPHbUoCXV7IE
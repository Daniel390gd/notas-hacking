
## Descripción 

There is some interesting information hidden around this site [http://mercury.picoctf.net:5080/](http://mercury.picoctf.net:5080/). Can you find it?
### pista

You should have enough hints to find the files, don't run a brute forcer.
## Solución

- Ingresamos a la pagina dada en la descripción.
![[03-Scavenger-Hunt_IMG1.png]]
- Inspeccionamos en la pagina y en el html viene una parte de la bandera.
![[03-Scavenger-Hunt_IMG2.png]]
- Viendo en el css viene la 2° parte de la bandera.
![[03-Scavenger-Hunt_IMG3.png]]
- Viendo el código javaSvcript no encontramos una parte de la bandera pero viene una pista.
- Con esa pista concluimos que debemos acceder al archivo robots.txt y efectivamente ahí viene otra parte de la bandera, además de otra pista para otra parte.
![[03-Scavenger-Hunt_IMG4.png]]
- La pista menciona apache por lo que en la URL quitamos el robots.txt y ponemos .htaccess, donde viene otra parte de la bandera y otra pista.
![[03-Scavenger-Hunt_IMG5.png]]
- Esta pista menciona algo sobre guardar información en Mac, investigando existe un archivo llamado .DS_Store que hace esto, por lo que reemplazamos el .htaccess por este archivo, obteniendo así la ultima parte de la bandera.
![[03-Scavenger-Hunt_IMG6.png]]



```
picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_35844447}
```

## Referencias

- https://youtu.be/E2gN3AGHirc?si=c5fgDiQ3oheQJInl

## Descripción 

[🥛](http://mercury.picoctf.net:48319/)
### pista

Look at the problem category
## Solución

- Vemos la imagen.
![[01-Milkslap_IMG1.png]]
- Inspeccionando el codigo buscamos la imagen.
- Encontramos el nombre de la imagen
![[01-Milkslap_IMG2.png]]
- Ponemos el nombre en la url y descargamos la imagen
![[01-Milkslap_IMG3.png]]
- Usamos zsteg -a para usar esteganografia y obtenemos la bandera.
![[01-Milkslap_IMG4.png]]




```
picoCTF{imag3_m4n1pul4t10n_sl4p5}
```

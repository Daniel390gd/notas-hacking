
## Descripción 

We found this [file](https://mercury.picoctf.net/static/09a86202e72dbdb5bf4d1b5d2c6a5b86/tunn3l_v1s10n). Recover the flag.
### pista

Weird that it won't display right...
## Solución

- Con wget descargamos el archivo.
![[04-tunn3l-v1s10n_IMG1.png]]
- Usando file vemos que el archivo son datos.
- Usando xxd vemos que su encabezado es BMP pero que esta incompleto., ademas vamos a cambiar la extensión del archivo a .bmp
![[04-tunn3l-v1s10n_IMG2.png]]
- Usando un editor hexadecimal modificamos el encabezado poniendo 28 en la posición 0E, de igual manera en el 0A colocamos 28.
![[04-tunn3l-v1s10n_IMG3.png]]
- Vemos que ya se puede ver la imagen pero no contiene la bandera.
![[04-tunn3l-v1s10n_IMG4.png]]
- Nos vamos al editor de nuevo y en el offset 16 cambiamos el valor para modificar el alto de la imagen.
![[04-tunn3l-v1s10n_IMG5.png]]
- Volvemos a abrir la imagen y podemos ver la bandera.
![[04-tunn3l-v1s10n_IMG6.png]]



```
picoCTF{qu1t3_a_v13w_2020}
```

## Referencias

- https://youtu.be/1ucy2G1PIh4?si=rVbYnJzp2WhdgIKi
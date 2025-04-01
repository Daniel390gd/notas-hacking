
## Descripción 

Find the flag in this [picture](https://jupiter.challenges.picoctf.org/static/89b371a46702a31aa9931a2a2b12f8bf/pico_img.png).
### pista

- What does meta mean in the context of files?
- Ever heard of metadata?
## Solución

- Con el comando wget descargamos la imagen.
![[02-So-Meta_IMG1.png]]
- Usamos el comando strings para buscar en los metadatos y vemos que esta la bandera.
![[02-So-Meta_IMG2.png]]



```
picoCTF{s0_m3ta_eb36bf44}
```

## Notas adicionales

Con exitfool podemos ver los metadatos de una imagen.

## Descripción 

Can you make sense of this file?Download the file [here](https://artifacts.picoctf.net/c/476/enc_flag).

### pista

Multiple decoding is always good.
## Solución

- Usando el comando wget descargamos el archivo.
![[Pasted image 20250218214232.png]]
-  Usando el comando cat vemos que el contenido esta en base 64, para decodificar se usa | base64 -d, lo haremos hasta que obtengamos la bandera.
![[Pasted image 20250218214827.png]]



```
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_4557ec3e}
```

## Notas adicionales


## Referencias



## Descripción 

This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?
### pista

- How do operating systems know what kind of file it is? (It's not just the ending!
- Make sure to submit the flag as picoCTF{XXXXX}

## Solución

- Con wget descargamos el archivo.
![[04-extensions_IMG1.png]]
- Cambiamos la extensión del archivo a png con el comando mv.
![[04-extensions_IMG2.png]]
- Usando eog al archivo flag.png obtenemos la bandera.
![[04-extensions_IMG3.png]]



```
picoCTF{now_you_know_about_extensions}
```

## Notas adicionales

Instalar eog para ver metadatos

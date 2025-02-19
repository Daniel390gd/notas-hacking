
## Descripción 

Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) without running it?

### pista

[strings](https://linux.die.net/man/1/strings)
## Solución

- Con el comando wget descargamos el archivo
![[Pasted image 20250218184519.png]]
- Con el comando strings extraemos las cadenas del archivo binario, ademas usaremos el grep para que muestre solo las cadenas que contengan la palabra pico.
![[Pasted image 20250218185205.png]]



```
picoCTF{5tRIng5_1T_d66c7bb7}
```

## Notas adicionales


## Referencias

- [strings(1) - Linux man page](https://linux.die.net/man/1/strings)


## Descripción 

Why use p and q when I can use more? Connect with `nc jupiter.challenges.picoctf.org 4557`.
### pista

There's more prime factors than p and q, finding d is going to be different.
## Solución

- Nos conectamos con nc a jupiter.challenges.picoctf.org 4557
- Nos dan 3 valores que son el de "c","e" y "n".
- Intentamos factorizar n pero no podemos determinar el valor de "p" y "q"
- Usando una calculadora como tal no nos da los valores pero calcula el totient n que es lo que necesitamos.
![[04-b00tl3gRSA3_IMG1.png]]
- Usando python calculamos la llave privada(d).
- Con eso podemos calcular m(texto plano).
- Usamos bytes.fromhex para obtener la bandera
![[04-b00tl3gRSA3_IMG2.png]]



```
picoCTF{too_many_fact0rs_4025135}
```


## Referencias

- [sig-ztdz-vfe (2025-05-22 12:05 GMT-6) - Google Drive](https://drive.google.com/file/d/1z9o-TNLp0iVIT2tME7-revA9iJjWrNee/view)
- [Integer factorization calculator](https://www.alpertron.com.ar/ECM.HTM)
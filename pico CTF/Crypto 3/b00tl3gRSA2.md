
## Descripción 

In RSA d is a lot bigger than e, why don't we use d to encrypt instead of e? Connect with `nc jupiter.challenges.picoctf.org 57464`.
### pista

What is e generally?
## Solución

- Nos conectamos con nc a jupiter.challenges.picoctf.org 57464`
- Nos dan valores, vemos que "e" tiene un valor muy grande.
- Usando python colocamos los valores en variables y para e en vez de usar el valor que se nos dio antes, usaremos su valor por defecto que es 65537.
- Calculamos m, esto ya que se equivocaron en los valores.
- Una vez con el valor de m usamos bytes.fromhex y obtenemos la bandera.
![[03-b00tl3gRSA2.png]]



```
picoCTF{bad_1d3a5_2152720}
```

## Referencias

- [sig-ztdz-vfe (2025-05-22 12:05 GMT-6) - Google Drive](https://drive.google.com/file/d/1z9o-TNLp0iVIT2tME7-revA9iJjWrNee/view)
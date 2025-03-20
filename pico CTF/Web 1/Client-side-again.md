
## Descripción 

Can you break into this super secure portal? `https://jupiter.challenges.picoctf.org/problem/60786/` ([link](https://jupiter.challenges.picoctf.org/problem/60786/)) or http://jupiter.challenges.picoctf.org:60786
### pista

- What is obfuscation?
## Solución

- Entramos a la pagina dada en la descripción.
![[06-Client-side-again_IMG1.png]]
- Inspeccionamos en la pagina y vemos que el código del método verify() esta ofuscado.
![[06-Client-side-again_IMG2.png]]
- Copiamos el código y usamos JS nice para desofuscarlo
![[06-Client-side-again_IMG3.png]]
- Tomamos la variable "_0x5a46" y la pegamos en la consola.
-  A partir del arreglo formamos la bandera.
![[06-Client-side-again_IMG4.png]]




```
picoCTF{not_this_again_ef49bf}
```

## Notas adicionales


## Referencias

- https://youtu.be/rsPT722MkzQ?si=smTDwdVayhgKZdsK
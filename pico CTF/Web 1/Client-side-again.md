
## Descripción 

Can you break into this super secure portal? `https://jupiter.challenges.picoctf.org/problem/60786/` ([link](https://jupiter.challenges.picoctf.org/problem/60786/)) or http://jupiter.challenges.picoctf.org:60786
### pista

- What is obfuscation?
## Solución

- Entramos a la pagina dada en la descripción.
![[Pasted image 20250319231342.png]]
- Inspeccionamos en la pagina y vemos que el código del método verify() esta ofuscado.
![[Pasted image 20250319231417.png]]
- Copiamos el código y usamos JS nice para desofuscarlo
![[Pasted image 20250319231855.png]]
- Tomamos la variable "_0x5a46" y la pegamos en la consola.
-  A partir del arreglo formamos la bandera.
![[Pasted image 20250319232420.png]]




```
picoCTF{not_this_again_ef49bf}
```

## Notas adicionales


## Referencias

- https://youtu.be/rsPT722MkzQ?si=smTDwdVayhgKZdsK
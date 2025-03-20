
## Descripción 

The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at? `https://jupiter.challenges.picoctf.org/problem/15796/` ([link](https://jupiter.challenges.picoctf.org/problem/15796/)) or http://jupiter.challenges.picoctf.org:15796
### pista

- Hmm it doesn't seem to check anyone's password, except for Joe's?
## Solución

- Entramos en la pagina dada por la descripción.
![[Pasted image 20250319230202.png]]
- Usamos como nombre de usuario admin y cualquier contraseña para intentar acceder.
![[Pasted image 20250319230245.png]]
- Observamos que aparece en la pagina que la bandera no esta disponible para nosotros.
![[Pasted image 20250319230328.png]]
- Vamos a inspeccionar y buscar las cookies, vemos que la de admin esta en "false" la modificamos a true.
![[Captura de pantalla 2025-03-19 230638.png]]
- Recargamos la pagina y vemos que ahora si aparece la bandera.
![[Captura de pantalla 2025-03-19 230649.png]]




```
picoCTF{th3_c0nsp1r4cy_l1v3s_6edb3f5f}
```

## Notas adicionales


## Referencias

- https://youtu.be/P2njyHWhu1U?si=WNelg-GggVbec7wL
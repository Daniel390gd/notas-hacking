
## Descripción 

Can you login to this website?Try to login [here](http://saturn.picoctf.net:58650/).
### pista

## Solución

- Ingresamos a la pagina dada en la descripción.
- Intentamos acceder usando admin como usuario y contraseña.
![[Pasted image 20250327124339.png]]
- Se nos indica que no se pudo.
![[Pasted image 20250327124356.png]]
- Hacemos una inyección sql.
![[Pasted image 20250327124321.png]]
- Vemos que la pagina dice que pudimos acceder, ahora inspeccionamos y vemos que en el html esta la bandera.
![[Pasted image 20250327124247.png]]
![[Pasted image 20250327124305.png]]


```
picoCTF{L00k5_l1k3_y0u_solv3d_it_9b0a4e21}
```


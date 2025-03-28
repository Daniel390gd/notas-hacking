
## Descripción 

Can you login to this website?Try to login [here](http://saturn.picoctf.net:58650/).
### pista

## Solución

- Ingresamos a la pagina dada en la descripción.
- Intentamos acceder usando admin como usuario y contraseña.
![[08-SQLiLite_IMG1.png]]
- Se nos indica que no se pudo.
![[08-SQLiLite_IMG2.png]]
- Hacemos una inyección sql.
![[08-SQLiLite_IMG3.png]]
- Vemos que la pagina dice que pudimos acceder, ahora inspeccionamos y vemos que en el html esta la bandera.
![[08-SQLiLite_IMG4.png]]
![[08-SQLiLite_IMG5.png]]


```
picoCTF{L00k5_l1k3_y0u_solv3d_it_9b0a4e21}
```


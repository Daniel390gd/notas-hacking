
## Descripción 

There's a flag shop selling stuff, can you buy a flag? [Source](https://jupiter.challenges.picoctf.org/static/64e724ad327f83ad833d9c6baa072b1f/store.c). Connect with `nc jupiter.challenges.picoctf.org 4906`.
### pista

Two's compliment can do some weird things when numbers get really big!
## Solución

- Ingresamos con el comando nc al servidor.
![[Pasted image 20250412192634.png]]
- Vemos que nos es imposible comprar la bandera, ya que tenemos 1100 y la bandera cuesta más.
- En la opción 1 hay una bandera que cuesta 900 y nos pide ingresar la cantidad de banderas a comprar al ingresar 100000000000000000 el balance aumenta.
![[Pasted image 20250412192824.png]]
- Compramos la bandera.
![[Pasted image 20250412192844.png]]



```
picoCTF{m0n3y_bag5_9c5fac9b}
```

## Referencias

- https://youtu.be/7qBamI8cFz0?si=y7dYduvP0s5rIJFe
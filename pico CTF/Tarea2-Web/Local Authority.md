
## Descripción 

Can you get the flag?Go to this [website](http://saturn.picoctf.net:62423/) and see what you can discover.
### pista

How is the password checked on this website?
## Solución

- Ingresamos en la pagina dada en la descripción.
- Intentamos acceder usando como usuario y contraseña admin.
![[Pasted image 20250327122131.png]]
- Vemos que nos manda a una pagina que dice que no pudimos acceder.
![[Pasted image 20250327122150.png]]
- Inspeccionando vemos que existe un archivo llamada secure.js y vemos que contiene una función llamada checkPassword que contiene la contraseña que necesitamos.
![[Pasted image 20250327122240.png]]
- Volvemos a la pagina principal y usamos la contraseña para obtener la bandera.
![[Pasted image 20250327122319.png]]



```
picoCTF{j5_15_7r4n5p4r3n7_05df90c8}
```

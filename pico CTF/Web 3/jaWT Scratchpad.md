
## Descripción 

Check the admin scratchpad! `https://jupiter.challenges.picoctf.org/problem/63090/` or http://jupiter.challenges.picoctf.org:63090
### pista

- What is that cookie?
- Have you heard of JWT?
## Solución

- Ingresamos a la pagina dada en la descripción.
- Si intentamos acceder con el nombre de usuario "admin" nos dice que no se puede.
![[03-JaWT-Scratchpad_IMG1.png]]
![[03-JaWT-Scratchpad_IMG2.png]]
- Accedemos con otro nombre, en mi caso Daniel
- ![[03-JaWT-Scratchpad_IMG3.png]]
- Al acceder se genera una cookie llamada jwt, esta la copiamos y pasamos a jwt.io para decodificarla.
![[03-JaWT-Scratchpad_IMG4.png]]
- Si intentamos cambiar el nombre de usuario a admin y cambiar el token al recargar no se podra, por lo que se tendra que borrar la cookie y recargar la pagina para acceder nuevamente y generar la cookie jwt de nuevo.
![[03-JaWT-Scratchpad_IMG5.png]]
![[03-JaWT-Scratchpad_IMG6.png]]
- En la terminal guardamos el token en un archivo
![[03-JaWT-Scratchpad_IMG7.png]]
- Vamos a desempaquetar un archivo para hacer un ataque de diccionario.
![[03-JaWT-Scratchpad_IMG8.png]]
- Usando john descubrimos que se uso la palabra ilovepico para firmar el token, vamos a poner esto en la firma y se genera un nuevo token.
![[03-JaWT-Scratchpad_IMG9.png]]
![[03-JaWT-Scratchpad_IMG10.png]]
- Volvemos a cambiar el valor de la cookie y recargamos, vemos que nos da la bandera
![[03-JaWT-Scratchpad_IMG11.png]]


```
picoCTF{jawt_was_just_what_you_thought_f859ab2f}
```


## Referencias

- https://youtu.be/iaKbvrbcSko?si=lp1DkPeoQ_OIxBBq
- https://jwt.io/
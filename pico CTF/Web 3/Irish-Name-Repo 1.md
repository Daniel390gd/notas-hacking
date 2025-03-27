
## Descripción 

There is a website running at `https://jupiter.challenges.picoctf.org/problem/50009/` ([link](https://jupiter.challenges.picoctf.org/problem/50009/)) or http://jupiter.challenges.picoctf.org:50009. Do you think you can log us in? Try to see if you can login!
### pista

- There doesn't seem to be many ways to interact with this. I wonder if the users are kept in a database?
- Try to think about how the website verifies your login.
## Solución

- Ingresamos a la pagina dada en la descripción.
- Buscamos la forma de interactuar.
- En el admin login intentamos ingresar usando admin como usuario y contraseña.
![[01-Irish-Name-Repo-1_IMG1.png]]
- Inspeccionando vemos que hay un campo llamado debug que es = 0, si le modificamos a 1 y intentamos volver a inicicar sesión muestra algo nuevo.
![[01-Irish-Name-Repo-1_IMG2.png]]

![[01-Irish-Name-Repo-1_IMG3.png]]

- Hacemos una inyección SQL
![[01-Irish-Name-Repo-1_IMG5.png]]
- Podemos ver que accedimos correctamente y obtenemos la bandera.
![[01-Irish-Name-Repo-1_IMG6.png]]



```
picoCTF{s0m3_SQL_fb3fe2ad}
```

## Referencias

- https://youtu.be/0EDbUSDqrng?si=yt7CzXrdW4oKr7dn
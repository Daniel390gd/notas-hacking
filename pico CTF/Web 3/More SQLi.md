
## Descripción 

Can you find the flag on this website.Try to find the flag [here](http://saturn.picoctf.net:59249/).
### pista

- SQLiLite
## Solución

- Ingresamos a la pagina dada en la descripción.
- Intentamos ingresar con admin como ususario y contraseña.
- Hacemos una inyección.
![[02-More-SQli_IMG1.png]]
- Como se puede ver se accedio a las tablas de la base de datos, ahora se buscara la contraseña, para esto primero verificaremos la versión usando un union select.
![[02-More-SQli_IMG2.png]]
- En este caso la versión es la 3.31.1
![[02-More-SQli_IMG3.png]]
- Usando ' union select sql,2,3 from sqlite_master; obtenemos la estructura de las tablas.
![[02-More-SQli_IMG4.png]]
- Vemos que la tabla "more_table" contiene un campo llamado flag, usaremos otra instrucción para obtener la bandera.
![[02-More-SQli_IMG5.png]]
![[02-More-SQli_IMG6.png]]


```
picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_e3e46aae}
```

## Referencias

- https://youtu.be/clMe4yqL6yU?si=Gcai994fCunMNYcb
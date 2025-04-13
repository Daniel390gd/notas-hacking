
## Descripción 


### pista

- Maybe try to find the JWT Signing Key ("secret key") in the source code? Maybe it's hardcoded somewhere? Or maybe try to crack it?
- The 'role' and 'userId' fields in the JWT can be of interest to you!
- The 'controllers', 'services' and 'security' java packages in the given source code might need your attention. We've provided a README.md file that contains some documentation.
- Upgrade your 'role' with the _new_ (cracked) JWT. And re-login for the new role to get reflected in browser's localStorage.
## Solución

- Entramos en la pagina.
![[07-Java-Code-Analysis!!_IMG1.png]]
- Accedemos con las credenciales que nos dan.
- Vemos que hauy un libro llamado flag que esta bloqueado.
![[07-Java-Code-Analysis!!_IMG2.png]]
- Si inspeccionamos vemos que se hacen varias solicitudes, estas tienen un token jwt.
![[07-Java-Code-Analysis!!_IMG3.png]]
- Viendo el codigo y la herramienta jwt.io modificamos el token.
![[07-Java-Code-Analysis!!_IMG4.png]]
- En el apartado de local storage ponemos el token modificado y los datos del usuario.
![[07-Java-Code-Analysis!!_IMG5.png]]
- Recargamos la pagina y ahora aparece la bandera.
![[07-Java-Code-Analysis!!_IMG6.png]]



```
picoCTF{w34k_jwt_n0t_g00d_7745dc02}
```

## Referencias

- https://youtu.be/AT61XquM3mI?si=RDdgVzzPEqhrDM3r
- https://jwt.io/
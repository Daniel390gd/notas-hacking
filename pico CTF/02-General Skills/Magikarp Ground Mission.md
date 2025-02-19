
## Descripción 

Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `ee388b88`

Additional details will be available after launching your challenge instance.

### pista

Finding a cheatsheet for bash would be really helpful!
## Solución

- Nos conectamos al servidor ssh indicado.
![[Pasted image 20250218213239.png]]
- Con el comando ls vemos los archivos y vemos que estan 2, al primero usando el comando cat obtenemos una parte de la bandera.
![[Captura de pantalla 2025-02-18 213550.png]]
- Usando cat en el otro archivo nos indica que tenemos que dirigirnos al directorio raiz, hecho esto listamos archivos y hay varios, de aqui solo 2 son importantes, uno de ellos usando cat nos da la segunda parte de la bandera.
![[Pasted image 20250218213907.png]]
- Usando cat en el archivo que nos da pista para la tercera parte nos indica que tenemos que dirigirnos al home usando ~, hecho esto listando archivos tenemos un archivo con la ultima parte, solamente usamos el cat y ya tenemos la bandera completa.
![[Pasted image 20250218214118.png]]



```
picoCTF{xxsh_0ut_0f_\/\/4t3r_3ca613a1}
```

## Notas adicionales


## Referencias



## Descripción 

Can you break into this super secure portal? `https://jupiter.challenges.picoctf.org/problem/29835/` ([link](https://jupiter.challenges.picoctf.org/problem/29835/)) or http://jupiter.challenges.picoctf.org:29835
### pista

- Never trust the client
## Solución

- Ingresamos a la pagina dada en la descripción.
![[04-dont-use-client-side_IMG1.png]]
- Vemos la pagina y inspeccionamos en busca de algo que nos ayude.
- Vemos que esta la bandera en una función llamada verify(), es decir que la contraseña del login de la pagina es la bandera.
![[04-dont-use-client-side_IMG2.png]]
- Unimos las distintas partes de la bandera.




```
picoCTF{no_clients_plz_7723ce}
```

## Notas adicionales

Basarse en los números para formar correctamente la bandera.
## Referencias

- 
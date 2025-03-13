
## Descripción 

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/11/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) in the same directory too.
### pista

- To view the file in the webshell, do: `$ nano level1.py`
- To exit `nano`, press Ctrl and x and follow the on-screen prompts.
- The `str_xor` function does not need to be reverse engineered for this challenge.
## Solución

- Con el comando wget descargamos en el mismo directorio la bandera y el password checker.
![[07-PW_Crack1_IMG1.png]]
- Si ejecutamos el archivo level1.py nos pide una contraseña, la cual no tenemos, por lo que usando el comando nano veremos el código, en busca de una pista.
- Observando el código vemos que la contr![[07-PW_Crack1_IMG2.png]]aseña es 1e1a.

- Volvemos a ejecutar y ingresamos la contraseña para obtener la bandera.
![[07-PW_Crack1_IMG3.png]]



```
picoCTF{545h_r1ng1ng_fa343060}
```

## Notas adicionales


## Referencias

- 
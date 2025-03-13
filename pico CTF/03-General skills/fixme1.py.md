
## Descripción 

Fix the syntax error in this Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/27/fixme1.py)
### pista

- Indentation is very meaningful in Python
- To view the file in the webshell, do: `$ nano fixme1.py`
- To exit `nano`, press Ctrl and x and follow the on-screen prompts.
- The `str_xor` function does not need to be reverse engineered for this challenge.
## Solución

- Con el comando wget descargamos el archivo fixme1.py
![[05-fixme1.py_IMG1.png]]
-  Al ejecutar el archivo vemos que marca error de indentación en la linea 20, por lo que para modificar el archivo usaremos el comando nano.
- Modificamos el archivo y guardamos los cambios.
![[05-fixme1.py_IMG2.png]]
- Volvemos a ejecutar el archivo y ahora si obtenemos la bandera.
![[05-fixme1.py_IMG3.png]]


```
picoCTF{1nd3nt1ty_cr1515_182342f7}
```

## Notas adicionales


## Referencias

- 
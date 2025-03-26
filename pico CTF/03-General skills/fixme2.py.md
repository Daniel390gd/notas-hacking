
## Descripción 

Fix the syntax error in the Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/4/fixme2.py)
### pista

- Are equality and assignment the same symbol?
- To view the file in the webshell, do: `$ nano fixme2.py`
- To exit `nano`, press Ctrl and x and follow the on-screen prompts.
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución

- Con el comando wget descargamos el archivo
![[06-fixme2.py_IMG1.png]]
- Lo ejecutamos y nos marca el siguiente error:
![[06-fixme2.py_IMG2.png]]
- Usando el comando nano vamos a modificar el archivo y guardar los cambios.
![[06-fixme2.py_IMG3.png]]
- Volvemos a ejecutar el archivo y obtenemos la bandera.
![[06-fixme2.py_IMG4.png]]


```
picoCTF{3qu4l1ty_n0t_4551gnm3nt_e8814d03}
```

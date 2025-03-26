
## Descripción 

Find the flag in the Python script![Download Python script](https://artifacts.picoctf.net/c/35/serpentine.py)
### pista

- Try running the script and see what happens
- In the webshell, try examining the script with a text editor like `nano`
- To exit `nano`, press Ctrl and x and follow the on-screen prompts.
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución

- Con wget descargamos el archivo python.
![[10-Serpentine_IMG1.png]]
-  Lo ejecutamos y vemos 3 opciones, si elegimos la opción b, al contrario de lo que dice no muestra la bandera.
![[10-Serpentine_IMG2.png]]
- Salimos del programa y ahora usaremos el comando nano para ver el contenido del archivo.
- Revisando el código vemos que existe una función llamada print_flag() que nunca se usa, modificamos el archivo y guardamos los cambios.
![[10-Serpentine_IMG3.png]]
-  Volvemos a ejecutar el archivo y obtenemos la bandera.
![[10-Serpentine_IMG4.png]]



```
picoCTF{7h3_r04d_l355_7r4v3l3d_ae0b80bd}
```


## Descripción 

Run the Python script `code.py` in the same directory as `codebook.txt`.

- [Download code.py](https://artifacts.picoctf.net/c/2/code.py)
- [Download codebook.txt](https://artifacts.picoctf.net/c/2/codebook.txt)
### pista

- On the webshell, use `ls` to see if both files are in the directory you are in
- The `str_xor` function does not need to be reverse engineered for this challenge.
## Solución

- Con el comando wget descargamos los archivos code.py y codebook.txt
- Usando el comando ls verificamos que esten descargados los 2 archivos en el mismo directorio.
![[03-Codebook_IMG1.png]]
- Ejecutamos el archivo code.py y obtenemos la bandera.
![[03-Codebook_IMG2.png]]



```
picoCTF{c0d3b00k_455157_7d102d7a}
```

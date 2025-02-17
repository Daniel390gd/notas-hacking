
## Descripción 

Unzip this archive and find the flag.

- [Download zip file](https://artifacts.picoctf.net/c/503/big-zip-files.zip)

### pista

Can grep be instructed to look at every file in a directory and its subdirectories?
## Solución

- Con wget descargamos el archivo .zip
- Utilizamos el comando unzip para descomprimirlo
- Utilizamos el comando grep con la opción -R para buscar la bandera entre archivos y directorios.
![[09-Big_Zip.png]]


```
picoCTF{gr3p_15_m4g1c_ef8790dc}
```

## Notas adicionales


## Referencias

- [Tutorial del comando Grep – Cómo buscar un archivo en Linux y Unix con búsqueda recursiva](https://www.freecodecamp.org/espanol/news/grep-command-tutorial-how-to-search-for-a-file-in-linux-and-unix-with-recursive-find/)

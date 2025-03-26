
## Descripción 

Unzip this archive and find the file named 'uber-secret.txt'
- [Download zip file](https://artifacts.picoctf.net/c/501/files.zip)

## Solución

- Con wget descargamos el archivo 'Files.zip'
- Usamos el comando unzip para descomprimir el archivo
![[10-First_Find_IMG1.png]]
- Con el comando find buscamos archivos con extensión .txt
![[10-First_Find_IMG2.png]]
- Ya teniendo la ruta del archivo usamos el comando Cat
![[10-First_Find_IMG3.png]]




```
picoCTF{f1nd_15_f457_ab443fd1}
```

## Referencias

- [Cómo encontrar un archivo en Linux desde la línea de comandos - Blog de SW Hosting](https://www.swhosting.com/es/blog/como-encontrar-un-archivo-en-linux-desde-la-linea-de-comandos)

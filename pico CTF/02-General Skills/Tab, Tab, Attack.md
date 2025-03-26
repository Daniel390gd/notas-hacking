
## Descripción 

Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: [Addadshashanammu.zip](https://mercury.picoctf.net/static/9689f2b453ad5daeb73ca7534e4d1521/Addadshashanammu.zip)

### pista

After `unzip`ing, this problem can be solved with 11 button-presses...(mostly Tab)...
## Solución

- Con el comando wget descargamos el archivo .zip
![[Pasted image 20250218212043.png]]
- Descomprimir el archivo con el comando unzip
![[Pasted image 20250218212250.png]]
- Usando el comando cd y la tecla |TAB| accedemos al ultimo directorio del archivo, vemos un archivo ejecutable, al ejecutarlo nos aparece la flag.
![[Pasted image 20250218212509.png]]



```
picoCTF{l3v3l_up!_t4k3_4_r35t!_2bcfb2ab}
```

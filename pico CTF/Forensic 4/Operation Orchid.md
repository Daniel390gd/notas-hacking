
## Descripción 

Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/213/disk.flag.img.gz)

## Solución

- Descargamos la imagen con wget y descomprimimos gon gzip -d.
![[05-Operation-Orchid_IMG1.png]]
- Usamos fls para ver donde estan los archivos.
![[05-Operation-Orchid_IMG2.png]]
- Usamos icat pero vemos que esta codificada la bandera.
![[05-Operation-Orchid_IMG3.png]]
- Guardamos la salida en un archivo y vemos como es que se codifico.
- Revertimos los comandos y usamos cat para obtener la bandera.
![[05-Operation-Orchid_IMG4.png]]



```
picoCTF{h4un71ng_p457_5113beab} 
```

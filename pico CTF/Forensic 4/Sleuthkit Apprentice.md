
## Descripción 

Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/137/disk.flag.img.gz)

## Solución

- con wget descargamos la imagen y usamos el comando gzip -d para desempaquetar.
![[04-Sleuthkit-Apprentice_IMG1.png]]
- Usando srch_strings y vemos que no esta la bandera.
- Usaremos fls para listar archivos.
![[04-Sleuthkit-Apprentice_IMG2.png]]
- Usamos icat para obtener la bandera.
![[04-Sleuthkit-Apprentice_IMG3.png]]



```
picoCTF{by73_5urf3r_adac6cb4}
```

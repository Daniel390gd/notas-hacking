
## Descripción 

Every file gets a flag.The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/260/flag.png).

## Solución

- Con wget descargamos la imagen.
![[04-hideme_IMG1.png]]
- Al abrirla vemos que no hay nada.
- Usamos unzip para descomprimir la imagen
- Vemos que se crea un directorio llamado secret y dentro de este esta un archivo llamado flag.png.
- Al abrirlo esta imagen contiene la bandera.
![[04-hideme_IMG2.png]]



```
picoCTF{Hiddinng_An_imag3_within_@n_ima9e_ad9f6587}
```

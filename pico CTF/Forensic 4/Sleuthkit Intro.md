
## Descripción 

Download the disk image and use mmls on it to find the size of the Linux partition. Connect to the remote checker service to check your answer and get the flag. Note: if you are using the webshell, download and extract the disk image into /tmp not your home directory. Download disk image Access checker program: nc saturn.picoctf.net 55465

## Solución

- Descargamos la imagen con wget.
- Descomprimimos con gzip -d.
![[03-Sleuthkit-Intro_IMG1.png]]
- Usamos el comando mmls.
![[03-Sleuthkit-Intro_IMG2.png]]
- Lanzamos la instancia y nos conectamos al servidor
- Nos hace una pregunta sobre el tamaño de una partición, con lo obtenido usando mmls la respondemos y obtenemos la bandera.
![[03-Sleuthkit-Intro_IMG3.png]]



```
picoCTF{mm15_f7w!}
```


## Descripción 

Can you abuse the banner?The server has been leaking some crucial information on `tethys.picoctf.net 60654`. Use the leaked information to get to the server.To connect to the running application use `nc tethys.picoctf.net 51387`. From the above information abuse the machine and find the flag in the /root directory.
### pista

- Do you know about symlinks?
- Maybe some small password cracking or guessing
## Solución

- Ingresamos al primer servidor y nos da unos datos
- Ingresamos al segundo servidor, donde nos pide una contraseña, esta viene en el primero, despues nos hace 2 preguntas una vez contestadas tenemos acceso.
![[07-dont-you-love-banners_IMG1.png]]
- Listamos archivos y hacemos cat al archivo banner y despues a uno llamado text
![[07-dont-you-love-banners_IMG2.png]]
- usando ls -al/root vemos que esta el archivo con la bandera y un archivo python.
![[07-dont-you-love-banners_IMG3.png]]
- Usamos cat en el archivo .py donde vienen indicaciones.
![[07-dont-you-love-banners_IMG4.png]]
- usamos el comando rm /home/player/banner
![[07-dont-you-love-banners_IMG5.png]]
- Usamos el comando ln -s /root/flag.txt /home/player/banner
![[07-dont-you-love-banners_IMG6.png]]
- Salimos del servidor y nos volvemos a conectar, podemos ver que nos despliega la bandera.
![[07-dont-you-love-banners_IMG7.png]]




```
picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_8126c9b0}
```

## Referencias

- https://youtu.be/M6N0IBIDp-Q?si=-XwRNaHI8thk9MMj
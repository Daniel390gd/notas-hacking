
## Descripción 

I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead? You can download the challenge files here:

    challenge.zip

The same files are accessible via SSH here: ssh -p 50373 ctf-player@atlas.picoctf.net Using the password 6dd28e9b. Accept the fingerprint with yes, and ls once connected to begin. Remember, in a shell, passwords are hidden!
### pista

- QR codes are a way of encoding data. While they're most known for storing URLs, they can store other things too.
- Mobile phones have included native QR code scanners in their cameras since version 8 (Oreo) and iOS 11
- If you don't have access to a phone, you can also use zbar-tools to convert an image to text
## Solución

- Descargamos con wget el archivo challenge.zip y usando unzip lo descomprimimos.
![[05-Scan-Surprise_IMG1.png]]
- Navegamos entre las carpetas hasta llegar a un archivo llamado flag.png, al abrirlo vemos un codigo QR.
![[05-Scan-Surprise_IMG2.png]]
- Usando una pagina para leer QR le pasamos el codigo y obtenemos la bandera.
![[05-Scan-Surprise_IMG3.png]]



```
picoCTF{p33k_@_b00_a81f0a35}
```

## Referencias

- https://youtu.be/tYxHqz47sww?si=Gq8rBOF6LkwV0hp6
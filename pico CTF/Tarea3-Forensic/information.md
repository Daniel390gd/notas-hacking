
## Descripción 

Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/7cf6a33f90deeeac5c73407a1bdc99b6/cat.jpg)
### pista

- Look at the details of the file
- Make sure to submit the flag as picoCTF{XXXXX}
## Solución

- Con wget descargamos el archivo cat.png
- Usamos el editor hexadecimal para ver metadatos.
![[01-information_IMG1.png]]
- Encontramos una cadena codificada en base64, con cyberchef la decodificamos y obtenemos la bandera.
![[01-information_IMG2.png]]



```
picoCTF{the_m3tadata_1s_modified}
```

## Referencias

- [CyberChef](https://cyberchef.org/)
- https://youtu.be/8a16UeEutD4?si=aGpGg7EYc93R_BTd

## Descripción 

RED, RED, RED, REDDownload the image: [red.png](https://challenge-files.picoctf.net/c_verbal_sleep/831307718b34193b288dde31e557484876fb84978b5818e2627e453a54aa9ba6/red.png)
### pista

- The picture seems pure, but is it though?
- Red?Ged?Bed?Aed?
- Check whatever Facebook is called now.
## Solución

- Con wget descargamos la imagen.
![[08-RED_IMG1.png]]
- Usamos zsteg --lsb --channel rgba y obtenemos una cadena de texto codificada en base 64.
![[08-RED_IMG2.png]]
- Usando cyberchef decodificamos la bandera.
![[08-RED_IMG3.png]]



```
picoCTF{r3d_1s_th3_ult1m4t3_cur3_f0r_54dn355_}
```

## Referencias

- [CyberChef](https://cyberchef.io/)
- https://youtu.be/tbJwWVW6wk8?si=qfLuthwOSRXDJglJ
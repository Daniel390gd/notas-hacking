
## Descripción 

The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?[Web Portal](http://saturn.picoctf.net:55643/)
### pista

XML external entity Injection
## Solución

- Entramos en la pagina dada por la descripción.
- Inspeccionamos la pagina en busca de pistas.
- Usamos Burp suite y vemos que las 3 peticiones hacen lo mismo.
![[02-SOAP_IMG1.png]]
- Usamos un payload para obtener la bandera.
![[02-SOAP_IMG2.png]]




```
picoCTF{XML_3xtern@l_3nt1t1ty_e79a75d4}
```

## Referencias

- https://youtu.be/b1pGlutUL34?si=SxgvvaHWpHztHPjY

## Descripción 

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.
### pista

- Try using a tool like Wireshark.
- How can you decrypt the TLS stream?
## Solución

- Usando wget descargamos los 2 archivos.
![[01-WebNet0_IMG1.png]]
- Usando wireshark si seguimos los stream TLS vemos que aparecen vacios.
- En preferencias nos vamos a protocolos y buscamos TLS, una vez hecho agreagamos la llave colocando el archivo .key que descargamos.
![[01-WebNet0_IMG2.png]]
- Vemos que ahora si aparece contenido en los streams.
- Buscamos la cadena picoCTF y vemos que esta la bandera.
![[01-WebNet0_IMG3.png]]



```
picoCTF{nongshim.shrimp.crackers}
```

## Referencias

- https://youtu.be/9uflLPoETOc?si=Mwd5WnUnN5ImpyOq
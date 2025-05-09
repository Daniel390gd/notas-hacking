
## Descripción 

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key). Recover the flag.
### pista

- Try using a tool like Wireshark.
- How can you decrypt the TLS stream?
## Solución

- Con el comando wget descargamos la captura de paquetes y la llave.
![[02-WebNet1_IMG1.png]]
- Usando wireshark nos vamos a preferencias, protocolos y buscamos TLS para poner la llave.
- Exportamos una imagen.
![[02-WebNet1_IMG2.png]]
- Abrimos esa imagen y no vemos nada, por lo que usando el comando strings vemos que hay esta la bandera.
![[02-WebNet1_IMG3.png]]



```
picoCTF{honey.roasted.peanuts}
```

## Referencias

- https://youtu.be/Ym3i79nEHjw?si=QV6Cf9o3l5rj-oN2

## Descripción 

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.

## Solución

- Con el comando wget descargamos la captura de paquetes.
![[05-shark-on-wire-2_IMG1.png]]
- Usamos wireshark para ver de que se trata.
![[05-shark-on-wire-2_IMG2.png]]
- Seguimos el stream de paquetes UDP
![[05-shark-on-wire-2_IMG3.png]]
- En el stream 32 viene "start" y en el 60 "end", vamos a filtrar aquellos paquetes cuyo puerto destino sea el 22, ya que estos streams mencionados comparten esa característica.
![[05-shark-on-wire-2_IMG4.png]]
- Verificamos que tengamos scapy.
![[05-shark-on-wire-2_IMG5.png]]
- Ya con scapy crearemos un exploit donde leemos los paquetes udp cuyo puerto destino sea 22, despues aquellos cuyo puerto destino sea mayor a 5000 nos los quedamos les restamos 5000 al puerto y convertir el resultado a ascii, imprimiendo al ultimo la bandera.
![[05-shark-on-wire-2_IMG6.png]]
- Ejecutamos el exploit y obtenemos la bandera.
![[05-shark-on-wire-2_IMG7.png]]



```
picoCTF{p1LLf3r3d_data_v1a_st3g0}
```


## Referencias

- https://youtu.be/WcMl1SvQ6hI?si=Oh0UAVYLSneLLd7f
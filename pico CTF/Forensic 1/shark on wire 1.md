
## Descripción 

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap). Recover the flag.
### pista

- Try using a tool like Wireshark
- What are streams?
## Solución

- Descargamos con wget el sniffer.
![[03-shark-on-wire-1_IMG1.png]]
- Usamos wireshark para ver los paquetes.
![[03-shark-on-wire-1_IMG2.png]]
- Tomamos un paquete UDP y damos en seguir stream, explorando en el stream 6 esta la bandera.
![[03-shark-on-wire-1_IMG3.png]]



```
picoCTF{picoCTF{StaT31355_636f6e6e}}
```


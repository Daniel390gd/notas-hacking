
## Descripción 

A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag.To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder!Find the PCAP file here [Network Traffic PCAP file](https://challenge-files.picoctf.net/c_verbal_sleep/a917f567b9cc0f1a730a7801b309955df4d2234a8114326857b9759e9e5d0453/myNetworkTraffic.pcap) and try to get the flag.
### pista

- Filter your packets to narrow down your search.
- Attacks were done in timely manner.
- Time is essential
## Solución

- Con el comando wget descargamos la captura de paquetes.
![[09-Ph4nt0m-1ntrud3r_IMG1.png]]
- Abrimos wireshark.
- Vamos a filtrar los paquetes con longitud 12.
![[09-Ph4nt0m-1ntrud3r_IMG2.png]]
- Vamos buscando en los paquetes filtrados las cadenas codificadas en base 64 y vamos formando la bandera.
![[09-Ph4nt0m-1ntrud3r_IMG3.png]]
![[09-Ph4nt0m-1ntrud3r_IMG4.png]]


```
picoCTF{1t_w4snt_th4t_34sy_tbh_4r_959f50d3}
```
## Referencias

- https://youtu.be/_YKC5Smffeg?si=Pfhsxz1ZI3FpYRbN
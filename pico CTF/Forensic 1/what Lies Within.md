
## Descripción 

There's something in the [building](https://jupiter.challenges.picoctf.org/static/011955b303f293d60c8116e6a4c5c84f/buildings.png). Can you retrieve the flag?
### pista

There is data encoded somewhere... there might be an online decoder.
## Solución

- Descargamos la imagen con wget.
![[05-what-Lies-Within_IMG1.png]]
- Usamos zsteg para usar estaganografia. y obtener la bandera.
![[05-what-Lies-Within_IMG2.png]]


```
picoCTF{h1d1ng_1n_th3_b1t5}
```

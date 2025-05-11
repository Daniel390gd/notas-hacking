
## Descripción 

We made a lot of substitutions to encrypt this. Can you decrypt it? Connect with `nc jupiter.challenges.picoctf.org 39894`.
### pista

Flag is not in the usual flag format
## Solución

- Nos conectamos con nc.
- Vemos que nos da un texto codificado.
![[07-waver-over-lambda_IMG1.png]]
- Utilizaremos quipqiup, le ponemos el texto y decodificamos.
- Vemos que el texto ya es entendible y obtenemos la bandera.
![[07-waver-over-lambda_IMG2.png]]



```
frequency_is_c_over_lambda_agflcgtyue
```

## Notas adicionales

La bandera no lleva el pico CTF{}
## Referencias

- [(5549) picoGym (picoCTF) Exercise: waves over lambda - YouTube](https://www.youtube.com/watch?v=y5uRI4rl6CI)
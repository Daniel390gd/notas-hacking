
## Descripción 

The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help `UFJKXQZQUNB` with the key of `SOLVECRYPTO`. Can you use this [table](https://jupiter.challenges.picoctf.org/static/1fd21547c154c678d2dab145c29f1d79/table.txt) to solve it?.
### pista

- Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{HELLO}' as the flag.
- Please use all caps for the message.
## Solución

- Descargamos la tabla con wget.
- La abrimos.
![[04-Easy-1_IMG1.png]]
- Vamos paso a paso decodificando usando la bandera encriptada y la llave.
![[04-Easy-1_IMG2.png]]
- Al final colocamos el texto dentro de las llaves.
![[04-Easy-1_IMG3.png]]



```
picoCTF{C R Y P T O I S F U N}
```

## Referencias

- https://youtu.be/ww1xjGR2C6w?si=46pG3gidJyQLp-20
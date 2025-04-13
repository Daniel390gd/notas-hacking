
## Descripción 

The Multiverse is within your grasp! Unfortunately, the server that contains the secrets of the multiverse is in a universe where keyboards only have numbers and (most) symbols.`ssh -p 58077 ctf-player@mimas.picoctf.net`Use password: `1ad5be0d`
### pista

Where can you get some letters?
## Solución

- Nos conectamos al servidor con ssh.
- Vemos que no podemos usar letras ni numeros solo wildcards.
- Usando diferentes wildcards vamos a acceder al archivo con la bandera.
![[Pasted image 20250412200130.png]]
- La bandera esta codificada en base 64 usando echo | base64 -d la decodificamos.
![[Pasted image 20250412200222.png]]



```
picoCTF{7h15_mu171v3r53_15_m4dn355_775ac12d}
```

## Notas adicionales


## Referencias

- https://youtu.be/ITTdaIh5mjA?si=5VU9apOhK3oq4KOE
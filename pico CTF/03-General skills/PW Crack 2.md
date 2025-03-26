
## Descripción 

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/14/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/14/level2.flag.txt.enc) in the same directory too.
### pista

- Does that encoding look familiar?
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución

- Con el comando wget descargamos la bandera y el password checker.
![[08-PW_Crack2_IMG1.png]]
-  Si ejecutamos el archivo level2.py vemos que como en el desafio PW Crack 1 pide un contraseña, nuevamente usamos nano para ver el archivo.
![[08-PW_Crack2_IMG2.png]]
- Vemos que la contraseña esta en hexadecimal, por lo que usaremos ciberchef con la receta From Hex para obtener la contraseña.
![[08-PW_Crack2_IMG3.png]]
- Sabiendo que la contraseña es 4ec9, volvemos a ejecutar el programa y ingresamos la contraseña para obtener la bandera.
![[08-PW_Crack2_IMG4.png]]



```
picoCTF{tr45h_51ng1ng_9701e681}
```

## Referencias

- [CyberChef](https://cyberchef.org/)
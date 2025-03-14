
## Descripción 

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/17/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/17/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.
### pista

- To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`
- To exit `bvi` type `:q` and press enter.
- The `str_xor` function does not need to be reverse engineered for this challenge.

## Solución

- Con el comando wget descargamos la bandera, el hash y el password checker.
![[09-PW-Crack3_IMG1.png]]
- Con el comando nano observamos el codigo del archivo level3.py, observamos hasta abajo que existen 7 posibles contraseñas.
![[09-PW-Crack3_IMG2.png]]
-  Para ver el hash usamos el comando bvi y el nombre del archivo.
![[09-PW-Crack3_IMG3.png]]
- Vemos el hash que es la contraseña encriptada, la tomamos y usamos hashes.com para ver si hay una coincidencia.
- Vemos que si hay una coincidencia y en este caso la contraseña es 87a.
![[09-PW-Crack3_IMG4.png]]
- Ejecutamos el archivo level3.py y ponemos la contraseña para obtener la bandera.
![[09-PW-Crack3_IMG5.png]]

### Solución 2
- Podemos ejecutar el programa level3.py y introducir una por una las 7 posibles contraseñas hasta encontrar la correcta.





```
picoCTF{m45h_fl1ng1ng_cd6ed2eb}
```

## Notas adicionales


## Referencias

- [Decrypt MD5, SHA1, MySQL, NTLM, SHA256, MD5 Email, SHA256 Email, SHA512, Wordpress, Bcrypt hashes for free online](https://hashes.com/en/decrypt/hash)

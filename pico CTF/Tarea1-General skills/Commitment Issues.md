
## Descripción 

I accidentally wrote the flag down. Good thing I deleted it!You download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/76/challenge.zip)
### pista

- Version control can help you recover files if you change or lose them!
- Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control)
- You can 'checkout' commits to see the files inside them

## Solución

- Con el comando wget descargamos el archivo.
- Con el comando unzip descomprimimos el archivo, quedando un archivo llamado drop in.
- Podemos ver que hay un archivo llamado message.txt que si usamos en el el comando cat dice que es secreto.
- Usaremos el comando git log para ver commits pasados.
![[04-Commitment_Issues_IMG1.png]]
- Podemos observar que existen 2 commits y en uno de ellos se creo la bandera, copiamos el id de ese commit.
- Ahora usaremos el comando git checkout y pegamos el id del commit.
![[04-Commitment_Issues_IMG2.png]]
- Volvemos a usar el comando cat en el archivo message.txt y observamos que nos da la bandera.
![[04-Commitment_Issues_IMG3.png]]


```
picoCTF{s@n1t1z3_7246792d}
```

## Notas adicionales

Verificar si se cuenta con git en el webshell.
## Referencias

- [The CTF Primer](https://primer.picoctf.org/#_git_version_control)
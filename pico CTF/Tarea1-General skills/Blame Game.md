
## Descripción 


### pista

- In collaborative projects, many users can make many changes. How can you see the changes within one file?
- Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
- You can use `python3 <file>.py` to try running the code, though you won't need to for this challenge.
## Solución

- Con el comando wget descargamos el archivo.
- Con el comando unzip descomprimimos el archivo.
- Una vez en el directorio usamos el comando git log para ver todos los commits.
- Vemos que el segundo commit fue realizado por un autor cuyo nombre tiene el formato de la bandera
![[06-Blame_Game.png]]



```
picoCTF{@sk_th3_1nt3rn_81e716ff}
```

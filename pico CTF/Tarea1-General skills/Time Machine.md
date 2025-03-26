
## Descripción 

What was I last working on? I remember writing a note to help me remember...You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/163/challenge.zip)
### pista

- The `cat` command will let you read a file, but that won't help you here!
- Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
- When committing a file with git, a message can (and should) be included.
## Solución

- Con el comando wget descargamos el archivo.
- Con el comando unzip descomprimimos el archivo.
- En drop-in vemos que tenemos un archivo llamado message.txt, si usamos el comando cat nos dice que veamos el historial de commits.
- Para hacer eso usaremos el comando git log.
- Podemos ver que hay un commit que contiene la bandera.
![[05-Time_Machine.png]]




```
picoCTF{t1m3m@ch1n3_88c35e3b}
```

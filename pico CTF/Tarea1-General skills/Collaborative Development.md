
## Descripción 

My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/70/challenge.zip)
### pista

- `git branch -a` will let you see available branches
- How can file 'diffs' be brought to the main branch? Don't forget to `git config`!
- Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim.

## Solución

- Con el comando wget descargamos el archivo
- Usando el comando unzip descomprimimos el archivo.
- En el directorio drop-in vemos un archivo llamado flag.py que si ejecutamos solo dice que se imprime la bandera pero en el código solo esta un print.
![[07-Collaborative-Development_IMG1.png]]
- Usaremos el comando git branch -a para ver las distintas ramas.
![[07-Collaborative-Development_IMG2.png]]
- Usaremos el comando git merge y pondremos uno por uno los nombres de las ramas.
![[07-Collaborative-Development_IMG3.png]]
- Al final tendremos en 3 partes la bandera, solamente las uniremos.
![[07-Collaborative-Development_IMG4.png]]



```
picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_7ffa0077}
```

## Referencias

- https://youtu.be/_CH5IQewkzw?si=aBJZwMPLP6TQLJ__
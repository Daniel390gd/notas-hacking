
## Descripción 

Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py) using [this password](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/pw.txt) to get [the flag](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/flag.txt.en)?
### pista

- Get the Python script accessible in your shell by entering the following command in the Terminal prompt: `$ wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py`
- $ man python
## Solución

- Usando el comando wget descargamos el script, la contraseña y la bandera.
![[Pasted image 20250412131251.png]]
- Usamos el comando cat para ver los archivos, el que nos interesa es la contraseña, ademas de ver que podemos ejecutar el script con las opciones -e,-d,-h.
- Ejecutamos el script con la opción -d y poniendo el archivo flag.txt
- Nos pedira la contraseña, copiamos y pegamos la contraseña del archivo pw.txt y obtenemos la bandera.
![[Pasted image 20250412132852.png]]


```
picoCTF{4p0110_1n_7h3_h0us3_aa821c16}
```


## Descripción 

Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/fc1d77192c544314efece5dd309092e3/warm) has extraordinarily helpful information...

### pista

- This program will only work in the webshell or another Linux computer.
- To get the file accessible in your shell, enter the following in the Terminal prompt: `$ wget https://mercury.picoctf.net/static/fc1d77192c544314efece5dd309092e3/warm`
- Run this program by entering the following in the Terminal prompt: `$ ./warm`, but you'll first have to make it executable with `$ chmod +x warm`
- -h and --help are the most common arguments to give to programs to get more information from them!
- Not every program implements help features like -h and --help.
## Solución

- Con el comando wget descargamos el binario
![[Pasted image 20250218185751.png]]
- Con el comando chmod le daremos permisos de ejecución
![[Pasted image 20250218185911.png]]
- Ejecutamos el programa con -h
![[Captura de pantalla 2025-02-18 190004.png]]




```
picoCTF{b1scu1ts_4nd_gr4vy_6635aa47}
```


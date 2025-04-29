
## Descripción 

Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/f6cc2560a70b1ea811c151accba5390f/dolls.jpg)
### pista

- Wait, you can hide files inside files? But how do you find them?
- Make sure to submit the flag as picoCTF{XXXXX}
## Solución

- Con el comando wget descargamos el archivo.
![[03-Matryoshka-doll_IMG1.png]]
- Usando binwalk vemos que hay un archivo dentro de la imagen.
![[03-Matryoshka-doll_IMG2.png]]
- Usando binwalk - e extraemos esa carpeta. dentro de esta hay otra carpeta que tiene una imagen de una matrioska.
- Repetimos el proceso, vemos con binwalk si hay archivos dentro de la imagen.
![[03-Matryoshka-doll_IMG3.png]]
- vemos que si hay por lo que descomprimmos, pero al final es algo parecido, por lo que repetimos el proceso.
- Vuelve a ocurrir lo mismo, por lo que repetimos proceso.
- Vemos que ahora hay un archivo llamado flag.txt, por lo que vamos a descomprimir.
![[03-Matryoshka-doll_IMG4.png]]
- Una vez descomprimido el archivo usamos cat para obtener la bandera del archivo flag.txt
![[03-Matryoshka-doll_IMG5.png]]



```
picoCTF{ac0072c423ee13bfc0b166af72e25b61} 
```
## Referencias

- https://youtu.be/NkbtA7x5aVI?si=9PzbL2o_rHUqMfka
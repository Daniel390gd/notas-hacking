
## Descripción 

The Network Operations Center (NOC) of your local institution picked up a suspicious file, they're getting conflicting information on what type of file it is. They've brought you in as an external expert to examine the file. Can you extract all the information from this strange file?Download the suspicious file [here](https://artifacts.picoctf.net/c_titan/98/flag2of2-final.pdf).
### pista

This problem can be solved by just opening the file in different ways
## Solución

- Descargamos la imagen con wget.
![[07-Secret-of-the-Polygot_IMG1.png]]
- Vemos que el archivo es una imagen png pero descargamos la imagen en formato pdf.
- Creamos una copia del archivo con extension png
- Abrimos la copia y obtenemos la primera parte de la bandera.
![[07-Secret-of-the-Polygot_IMG2.png]]
- Abriendo el archivo original obtenemos la otra parte.
![[07-Secret-of-the-Polygot_IMG3.png]]



```
picoCTF{f1u3n7_1n_pn9_&_pdf_1f991f77}
```
## Referencias

- https://youtu.be/F2NbpA4FgdY?si=r37txDdGngqBdsQt
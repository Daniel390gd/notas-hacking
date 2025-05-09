
## Descripción 

I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/c00c449c3b08daaccacca6f9d5c55d49/Forensics%20is%20fun.pptm)
## Solución

- Usamos wget para descargar el archivo.
![[05-MacroHard-WeakEdge_IMG1.png]]
- Usando file vemos que es un archivo .PPTM y investigando vemos que se puede descomprimir, por lo que usaremos el comando unzip.
![[05-MacroHard-WeakEdge_IMG2.png]]
- Instalamos VS code para visualizar los archivos.
![[05-MacroHard-WeakEdge_IMG3.png]]
- Buscando encontramos un archivo llamado hidden que contiene una cadena de texto en base 64.
![[05-MacroHard-WeakEdge_IMG4.png]]
- Usando ciberchef con la receta From Base64 obtenemos la bandera.
![[05-MacroHard-WeakEdge_IMG5.png]]



```
picoCTF{D1d_u_kn0w_ppts_r_z1p5}
```

## Referencias

- https://youtu.be/CsCeOp9PFGs?si=xV1RecHIo0IJtfLY
- [CyberChef](https://cyberchef.io/)
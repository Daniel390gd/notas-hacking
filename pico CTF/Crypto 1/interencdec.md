
## Descripción 

Can you get the real meaning from this file.Download the file [here](https://artifacts.picoctf.net/c_titan/109/enc_flag).
### pista

Engaging in various decoding processes is of utmost importance
## Solución

- Con wget descargamos el archivo.
- Usando cat vemos que es una cadena codificada en base 64.
![[08-interencdec_IMG1.png]]
- Usando cyberchef obtenemos otra cadena en base 64 codificada.
![[08-interencdec_IMG2.png]]
- A esta cadena le quitamos las comillas y la b y obtenemos otra cadena cifrada con cesar.
![[08-interencdec_IMG3.png]]
- Usando en decodificador de cifrado cesar obtenemos la bandera.
![[08-interencdec_IMG4.png]]



```
picoCTF{caesar_d3cr9pt3d_f0212758}
```
## Referencias

- [Cifrado César Traductor - Cifrar/Descifrar Codigo Cesar Online](https://www.dcode.fr/cifrado-cesar)
- [CyberChef](https://cyberchef.org/)
- https://youtu.be/lqltY8ZNH2o?si=AXZdmvIWzxZVMcox
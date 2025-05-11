
## Descripción 

How about some hide and seek?Download this file [here](https://artifacts.picoctf.net/c_titan/4/unknown.zip).
### pista

- How can you view the information about the picture?
- If something isn't in the expected form, maybe it deserves attention?
## Solución

- Con wget descargamos el archivo y usando unzip lo descomprimimos.
- Usando exiftool obtenemos una cadena codificada en base 64
![[06-CanYouSee_IMG1.png]]
- Decodificamos la cadena usando cyberchef y obtenemos la bandera.
![[06-CanYouSee_IMG2.png]]



```
picoCTF{ME74D47A_HIDD3N_deca06fb}
```


## Referencias

- https://youtu.be/1e8fCdTxijQ?si=Xug0JaYDCP7CMt0S
- [CyberChef](https://cyberchef.org/)

## Descripción 

Now you DON’T see me.This [report](https://artifacts.picoctf.net/c/84/Financial_Report_for_ABC_Labs.pdf) has some critical data in it, some of which have been redacted correctly, while some were not. Can you find an important key that was not redacted properly?
### pista

How can you be sure of the redaction?
## Solución

- Con wget descargamos la imagen.
- La abrimos y vemos que hay datos censurados.
![[03-Redaction-gone-wrong_IMG1.png]]
- Si observamos bien se selecciona todo, por lo que copiamos y pegamos en otra parte.
- Obtenemos la bandera.
![[03-Redaction-gone-wrong_IMG2.png]]



```
picoCTF{C4n_Y0u_S33_m3_fully}
```


## Referencias

- [(5562) picoGym (picoCTF) Exercise: Redaction gone wrong - YouTube](https://www.youtube.com/watch?v=VZNW2XXQZkM)

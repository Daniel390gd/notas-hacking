
## Descripción 

The flag is somewhere on this web application not necessarily on the website. Find it.Check [this](http://saturn.picoctf.net:62027/) out.

## Solución

- Ingresamos en la pagina dada por la descripción.
- Por el nombre del reto vamos a checar el archivo robots .txt
![[06-Roboto-Sans_IMG1.png]]
- Vemos que hay un texto en base 64, decodificandolo tenemos lo siguiente.
![[06-Roboto-Sans_IMG2.png]]
- Quitando 2 lineas aparece el nombre de un archivo.
![[06-Roboto-Sans_IMG3.png]]
- Ponemos este en la ruta y obtenemos la bandera.
![[06-Roboto-Sans_IMG4.png]]



```
picoCTF{Who_D03sN7_L1k5_90B0T5_718c9043}
```

## Referencias

- [CyberChef](https://cyberchef.org/)
- https://youtu.be/BBkhYcdKBLE?si=Tf11pMeD5DtD405-

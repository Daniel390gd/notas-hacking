
## Descripción 

Do you know how to use the web inspector?Start searching [here](http://titan.picoctf.net:62069/) to find the flag
### pista

- Use the web inspector on other files included by the web page.
- The flag may or may not be encoded
## Solución

- Entramos en la pagina dada en la descripción.
- Navegamos por la pagina inspeccionando, en la pagina de "about" dice que puede estar la bandera.
![[10-Web-Decode_IMG1.png]]
- Viendo el html hay una cadena en base 64.
![[10-Web-Decode_IMG2.png]]
- Usando ciberchef con la receta "From Base64" decodificamos el texto y obtenemos la bandera.
![[10-Web-Decode_IMG3.png]]



```
picoCTF{web_succ3ssfully_d3c0ded_f6f6b78a}
```

## Referencias

- [CyberChef](https://cyberchef.org/)
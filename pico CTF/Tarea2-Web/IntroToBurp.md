
## Descripción 

Try [here](http://titan.picoctf.net:59143/) to find the flag
### pista

- Try using burpsuite to intercept request to capture the flag.
- Try mangling the request, maybe their server-side code doesn't handle malformed requests very well.
## Solución

- Ingresamos a la pagina dada en la descripción usando burp suite.
- Llenamos los datos del formulario con cualquier cosa y en burp suite le damos en la opción forward.
![[03-IntroToBurp_IMG1.png]]
- Ahora pide un factor de autenticación, si ponemos cualquier cosa no obtendremos el acceso, pero si vemos abajo en la petición se genero el otp=test, si lo borramos y damos a forward la pagina nos dara la bandera.
![[03-IntroToBurp_IMG2.png]]
![[03-IntroToBurp_IMG3.png]]
![[03-IntroToBurp_IMG4.png]]


```
picoCTF{#0TP_Bypvss_SuCc3$S_e1eb16ed}
```

## Referencias

- [Bing Vídeos](https://www.bing.com/videos/riverview/relatedvideo?&q=instalar+burp+suite+kali+linux&&mid=A1A696C13244398327A0A1A696C13244398327A0&&FORM=VRDGAR)
- https://youtu.be/VU3yheDrODI?si=4YWP2sSMOlwv3AGK
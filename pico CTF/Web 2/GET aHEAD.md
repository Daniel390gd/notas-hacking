
## Descripción 

Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:47967/](http://mercury.picoctf.net:47967/)
### pista

- Maybe you have more than 2 choices
- Check out tools like Burpsuite to modify your requests and look at the responses
## Solución

- Ingresar a la pagina dada en la descripción.
![[01-GET-aHEAD_IMG1.png]]
- Inspeccionando el código no vemos nada fuera de lo normal, asi que nos vamos al apartado de red y vamos a hacer una solicitud pulsando en rojo o en azul.
![[01-GET-aHEAD_IMG2.png]]
- Vemos que el método del request es POST, lo cambiaremos a HEAD.
![[01-GET-aHEAD_IMG3.png]]
- Vemos en los datos generales del request la bandera.
![[01-GET-aHEAD_IMG4.png]]



```
picoCTF{r3j3ct_th3_du4l1ty_cca66bd3}
```

## Notas adicionales

En mi navegador al mandar el request con el método HEAD me salia que la URL estaba bloqueada, lo que hice fue dar click derecho a ese request y poner la opción unbloc url, posteriormente le di nuevamente click derecho y le di a la opción edit & resend.
## Referencias

- https://youtu.be/oiZk0tIkR48?si=sobSJAbui2AUlIwj
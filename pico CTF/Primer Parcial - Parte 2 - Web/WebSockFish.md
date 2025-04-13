
## Descripción 

Can you win in a convincing manner against this chess bot? He won't go easy on you!You can find the challenge [here](http://verbal-sleep.picoctf.net:54668/).
### pista

Try understanding the code and how the websocket client is interacting with the server
## Solución

- Entramos en la pagina.
![[10-WebSockFish_IMG1.png]]
- Si jugamos vemos que no es posible ganar, por lo que vamos a inspeccionar el código fuente en busca de algo que nos ayude.
- Encontramos un webSocket por lo que podemos enviar mensajes a traves de la consola.
![[10-WebSockFish_IMG2.png]]
- Con la función sendMessage podemos mandar mensajes y cambia el dialogo del pez.
![[10-WebSockFish_IMG3.png]]
- Usamos numeros negativos y vemos que pasa.
![[10-WebSockFish_IMG4.png]]
- El pez nos dio la bandera.




```
picoCTF{c1i3nt_s1d3_w3b_s0ck3t5_50441bef}
```

## Referencias

- https://youtu.be/xqopwb8Iv90?si=l2lbv4MO4sFHyRLD
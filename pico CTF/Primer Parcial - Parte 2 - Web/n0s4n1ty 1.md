
## Descripción 

A developer has added profile picture upload functionality to a website. However, the implementation is flawed, and it presents an opportunity for you. Your mission, should you choose to accept it, is to navigate to the provided web page and locate the file upload area. Your ultimate goal is to find the hidden flag located in the `/root` directory.You can access the web application [here](http://standard-pizzas.picoctf.net:64079/)!
### pista

- File upload was not sanitized
- Whenever you get a shell on a remote machine, check `sudo -l`
## Solución

- Entramos en la pagina.
![[04-n0s4n1ty-1_IMG1.png]]
- Vemos que podemos subir imagenes y acceder a la ruta donde se suben estas.
- Vamos a usar locate para copiar un backdoor que subiremos a la pagina.
![[04-n0s4n1ty-1_IMG2.png]]
- Lo subimos a la pagina y vemos que no hay seguridad y podemos ejecutar comandos.
![[04-n0s4n1ty-1_IMG3.png]]
![[04-n0s4n1ty-1_IMG4.png]]
- Usando sudo cat /root/flag.txt obtenemos la bandera.
![[04-n0s4n1ty-1_IMG5.png]]



```
picoCTF{wh47_c4n_u_d0_wPHP_f7424fc7}
```

## Referencias

- https://youtu.be/RawY672j488?si=WfR69CJPnP4pnBB3
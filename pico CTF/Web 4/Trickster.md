
## Descripción 

I found a web app that can help process images: PNG images only!Try it [here](http://atlas.picoctf.net:57474/)!
## Solución

- Entramos en la pagina dada en la descripción.
- Buscamos en el archivo robots.txt, vemos que podemos acceder a lo que subamos con /uploads/ y que hay un archivo con instrucciones.
![[03-Trickster_IMG1.png]]
- Vemos el archivo con instrucciones, con este usaremos un webshell de php con la extensión.png.
![[03-Trickster_IMG2.png]]
![[03-Trickster_IMG3.png]]
- Lo subimos y verificamos que se suba correctamente.

- nos vamos a /uploads para que se ejecute el archivo y usamos un ls para ver si se ejecuta código ademas de ver donde estamos.
![[03-Trickster_IMG4.png]]
- Una vez que vemos que si se ejecuta vamos buscando la bandera, la cual esta en un archivo de nombre raro.
![[03-Trickster_IMG5.png]]
![[03-Trickster_IMG6.png]]



```
picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_03d1d548}
```

## Referencias

- https://youtu.be/co8MZmviC1U?si=uaB1L_XJB6ZdZZyI
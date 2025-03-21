
## Descripción 

Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:27177/](http://mercury.picoctf.net:27177/)

## Solución

- Ingresamos a la pagina dada en la descripción.
![[02-Cookies_IMG1.png]]
- Vemos que podemos ir cambiando el valor de la cookie pero esto es muy lento.
- Para "automatizarlo" podemos usar un ciclo for en la terminal haciendo que se ejecute el comando curl con las opciones -s y -H, ademas de usar el comando grep para obtener la bandera.
![[02-Cookies_IMG2.png]]



```
picoCTF{3v3ry1_l0v3s_c00k135_064663be}
```

## Notas adicionales


## Referencias

- https://youtu.be/LseQ-XWCXVo?si=_z0pT-4r9S1HRYZM
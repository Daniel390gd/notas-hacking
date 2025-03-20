
## Descripción 

This website can be rendered only by **picobrowser**, go and catch the flag! `https://jupiter.challenges.picoctf.org/problem/50522/` ([link](https://jupiter.challenges.picoctf.org/problem/50522/)) or http://jupiter.challenges.picoctf.org:50522
### pista

- You don't need to download a new web browser
## Solución

- Entramos a la pagina dada en la descripción.
![[05-picobrowser_IMG1.png]]
- Presionamos el botón flag y nos sale lo siguiente:
![[05-picobrowser_IMG2.png]]
- Inspeccionando vemos las request y vemos los de flag.
- Cambiamos el valor de user-Agent a picobrowser.
- Checamos el request y le damos a response
- Ya tenemos la bandera.
![[05-picobrowser_IMG3.png]]



```
picoCTF{p1c0_s3cr3t_ag3nt_51414fa7}
```

## Notas adicionales

Las primeras 2 imágenes fueron en el navegador Edge pero como no encontré forma de modificar el user-Agent opte por hacerlo en mi maquina virtual usando otro navegador
## Referencias

- https://youtu.be/9d6-N0oJwOk?si=saaptAsQMfhQGGHY
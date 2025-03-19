
## Descripción 

Welcome to the challenge! In this challenge, you will explore a web application and find an endpoint that exposes a file containing a hidden flag.The application is a simple blog website where you can read articles about various topics, including an article about API Documentation. Your goal is to explore the application and find the endpoint that generates files holding the server’s memory, where a secret flag is hidden.The website is running [picoCTF News](http://verbal-sleep.picoctf.net:53822/).
### pista

- Explore backend development with us
- The head was dumped.
## Solución

- Observamos la pagina y nos vamos a un "apartado que dice "Explore backend development with us"
![[Pasted image 20250315185333.png]]
- Entre los links que tiene hay uno que dice #API Documentation, le damos click.
- En la pagina que nos cargo vemos algunas funciones, nos vamos hasta abajo en la que dice "Diagnosing".
![[Pasted image 20250315185508.png]]
- Le damos al boton Try it out y a execute.
- Descargamos el archivo.
![[Pasted image 20250315185640.png]]
- Abrimos el archivo y en el buscamos la bandera.
![[Pasted image 20250315185704.png]]





```
picoCTF{Pat!3nt_15_Th3_K3y_388d10f7}
```

## Notas adicionales


## Referencias

- 
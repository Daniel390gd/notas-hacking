
## Descripción 

Can you get the flag?Go to this [website](http://saturn.picoctf.net:58257/) and see what you can discover.
### pista

Is there more code than what the inspector initially shows?
## Solución

- Ingresamos a la pagina dada en la descripción.
- Inspeccionamos los archivos html, css y js
- Vemos que en el archivo css esta la primera parte de la bandera.
![[Pasted image 20250327123720.png]]
- En el archivo js viene la otra parte de la bandera, solamente queda juntar las partes.
![[Pasted image 20250327123732.png]]



```
picoCTF{1nclu51v17y_1of2_f7w_2of2_6edef411}
```


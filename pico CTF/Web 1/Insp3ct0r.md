
## Descripción 

Kishor Balan tipped us off that the following code may need inspection: `https://jupiter.challenges.picoctf.org/problem/44924/` ([link](https://jupiter.challenges.picoctf.org/problem/44924/)) or http://jupiter.challenges.picoctf.org:44924
### pista

- How do you inspect web code on a browser?
- There's 3 parts
## Solución

- Ingresamos a la pagina dada en la descirpción.
![[Pasted image 20250319082331.png]]
- Damos click derecho y buscamos la opción que dice "inspeccionar".
![[Pasted image 20250319082348.png]]
- Observamos el código html y vemos que esta comentada una parte de la bandera.
![[Pasted image 20250319082522.png]]
- Nos vamos a la pestaña de fuentes y vemos otros 2 archivos a parte del html.
![[Pasted image 20250319082615.png]]
- Buscamos en otro archivo y en este caso obtuve del archivo myjs.js la 3° parte de la bandera.
![[Pasted image 20250319082707.png]]
- Revisamos el archivo mycss.css y vemos que tiene la 2° parte de la bandera.
- Unimos las 3 partes.





```
picoCTF{tru3_d3t3ct1ve_0r_ju5t_lucky?f10be399}
```

## Notas adicionales


## Referencias

- 

## Descripción 

If you want to hash with the best, beat this test!`nc saturn.picoctf.net 61646`
### pista

- You can use a commandline tool or web app to hash text
- Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
## Solución

- Usamos el comando nc para conectarnos.
- Nos pide poner como un hash md5 la palabra computer hackers, para esto nos vamos a ciberchef y usamos la receta MD5.
![[02-HashingJobApp_IMG1.png]]
- Una vez ingresado y correcto, ahora nos pide hashear la palabra "leeches"
![[02-HashingJobApp_IMG2.png]]
- Por ultima vez nos pide hashear una palabra, babies en este caso.
![[02-HashingJobApp_IMG3.png]]
- Una vez correcta la 3° palabra nos da la bandera.
![[02-HashingJobApp_IMG4.png]]



```
picoCTF{4ppl1c4710n_r3c31v3d_674c1de2}
```

## Referencias

- [CyberChef](https://cyberchef.org/)
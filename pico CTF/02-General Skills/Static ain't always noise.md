
## Descripción 

Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/static)? This [BASH script](https://mercury.picoctf.net/static/ec4dbd8898ade34e1d60d5b70c1b8c8c/ltdis.sh) might help!

## Solución

- Con el comando wget descargamos los 2 archivos.
![[Pasted image 20250218190440.png]]
- Le damos permiso de ejecución al archivo "static" y ejecutamos.
![[Pasted image 20250218190742.png]]
- Ejecutamos el comando bash con el nombre del segundo archivo y posteriormente ponemos static(nombre del primer archivo)
![[Pasted image 20250218191056.png]]
- Para los 2 archivos generados usamos cat para ver su contenido
![[Pasted image 20250218191349.png]]



```
picoCTF{d15a5m_t34s3r_98d35619}
```

## Notas adicionales

En el ultimo paso sería mas optimo usar el comando grep pero como alcance a ver la flag se omitió el comando.
## Referencias


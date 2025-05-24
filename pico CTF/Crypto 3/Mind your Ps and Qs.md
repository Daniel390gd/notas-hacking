
## Descripción 

In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/51d68e61bb41207a55f24e753f07c5a3/values)
### pista

Bits are expensive, I used only a little bit over 100 to save money
## Solución

- Con wget descargamos el archivo con los valores.
- Vemos que n es un valor "pequeño" por lo que podemos intentar factorizarlo para obtener "p" y "q"
- Usando factordb encontramos valores para "p" y "q"
![[02-Mind-your-Ps-and-Qs_IMG1.png]]
- Ya con esos valores calculamos el totien n(tn).
- Una vez calculado calculamos la llave privada(d).
- Ya con esta podemos calcular m(texto plano).
- Finalmente usando bytes.fromhex obtenemos la bandera.
![[02-Mind-your-Ps-and-Qs_IMG2.png]]



```
picoCTF{small_N_n0_g0od_05012767}
```

## Referencias

- [sig-ztdz-vfe (2025-05-22 12:05 GMT-6) - Google Drive](https://drive.google.com/file/d/1z9o-TNLp0iVIT2tME7-revA9iJjWrNee/view)
- [factordb.com](http://www.factordb.com/)

## Descripción 

What happens if you have a small exponent? There is a twist though, we padded the plaintext so that (M ** e) is just barely larger than N. Let's decrypt this: [ciphertext](https://mercury.picoctf.net/static/81689952b7442c3e23a9f703198c0a4c/ciphertext)
### pista

- RSA [tutorial](https://en.wikipedia.org/wiki/RSA_\(cryptosystem\))
- How could having too small of an `e` affect the security of this key?
- Make sure you don't lose precision, the numbers are pretty big (besides the `e` value)
- You shouldn't have to make _too_ many guesses
- `pico` is in the flag, but not at the beginning
## Solución

- Con wget descargamos el texto cifrado.
![[01-Mini-RSA_IMG1.png]]
- Creamos un exploit que hará aproximaciones.
![[01-Mini-RSA_IMG2.png]]
- Utilizamos el exploit y con este obtenemos la bandera.
![[01-Mini-RSA_IMG3.png]]



```
picoCTF{e_sh0u1d_b3_lArg3r_7adb35b1}
```

## Referencias

- [sig-ztdz-vfe (2025-05-22 12:05 GMT-6) - Google Drive](https://drive.google.com/file/d/1z9o-TNLp0iVIT2tME7-revA9iJjWrNee/view)

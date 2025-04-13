
## Descripción 

Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag!Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/dcdaf491b35c1d0f5075e9583edbbb7aaea1dffb6ad32bc000e4d87b5200ff7b/fixme3.tar.gz).
### pista

Read the comments...darn it!
## Solución

- Descargamos el codigo.
- vemos que en los comentarios indica algo sobre funciones inseguras, por lo que nos vamos al link de la documentación.
- Modificamos la operación insegura con "unsafe {}"
- Ejecutamos el código y obtenemos la bandera.
![[06-Rust-fixme-3.png]]



```
picoCTF{n0w_y0uv3_f1x3d_1h3m_411}
```

## Referencias

- [Unsafe Rust - The Rust Programming Language](https://doc.rust-lang.org/book/ch20-01-unsafe-rust.html)
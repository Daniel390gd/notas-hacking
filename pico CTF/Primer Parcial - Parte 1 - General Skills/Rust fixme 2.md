
## Descripción 

The Rust saga continues? I ask you, can I borrow that, pleeeeeaaaasseeeee?Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/babfbee79718a6363826ba86300173ffde6d81577e9dd07d4130c53a7eecf6c3/fixme2.tar.gz).
### pista

https://doc.rust-lang.org/book/ch04-02-references-and-borrowing.html
## Solución

- Descargamos el código.
- Vemos que marca errores en "borrowed_string"
- cambiamos `borrowed_string: &String` por `borrowed_string: &mut String` para permitir modificaciones.
- Ejecutamos el código y obtenemos la bandera.
![[05-Rust-fixme-2.png]]



```
picoCTF{4r3_y0u_h4v1n5_fun_y31?}
```

## Referencias

- [References and Borrowing - The Rust Programming Language](https://doc.rust-lang.org/book/ch04-02-references-and-borrowing.html)
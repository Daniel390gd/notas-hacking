
## Descripción 

Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag!Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme1.tar.gz).

### pista

- Cargo is Rust's package manager and will make your life easier. See the getting started page [here](https://doc.rust-lang.org/book/ch01-03-hello-cargo.html)
- [println!](https://doc.rust-lang.org/std/macro.println.html)
- Rust has some pretty great compiler error messages. Read them maybe?

## Solución

- Instalamos el archivo, en mi caso extraje la carpeta y la moví a otra ubicación:
- Instalamos Rust para windows
- En visual Studio Code se instalarón extensiones para Rust (Rust analyzer y Code LLB).
- Modificamos el formato de salida de la función println con las llaves "{}"
- En otra parte del programa quitamos la variable ret y lo reemplazaremos por std::process::exit(1);



```
picoCTF{4r3_y0u_4_ru$t4c30n_n0w?}
```

## Notas adicionales

- Se puede instalar el Visual Studio Code(Morado), pero de no hacerlo se puede cambiar al toolchain de GNU para evitar problemas a la hora de compilar 
## Referencias

- [println in std - Rust](https://doc.rust-lang.org/std/macro.println.html)

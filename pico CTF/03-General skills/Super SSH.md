
## Descripción 

Using a Secure Shell (SSH) is going to be pretty important.Can you `ssh` as `ctf-player` to `titan.picoctf.net` at port `50102` to get the flag?You'll also need the password `6abf4a82`. If asked, accept the fingerprint with `yes`.If your device doesn't have a shell, you can use: [https://webshell.picoctf.org](https://webshell.picoctf.org/)If you're not sure what a shell is, check out our Primer: [https://primer.picoctf.com/#_the_shell](https://primer.picoctf.com/#_the_shell)
### pista

- [https://linux.die.net/man/1/ssh](https://linux.die.net/man/1/ssh)
- You can try logging in 'as' someone with `<user>`@titan.picoctf.net
- How could you specify the port?
- Remember, passwords are hidden when typed into the shell
## Solución

Usando el comando ssh con la opción -p nos conectamos a `titan.picoctf.net` como el usuario ctf-player.
Vemos que nos pide la contraseña, la cual viene en la descripción del desafio, la ingresamos y obtenemos la bandera.
![[01-Super-SSH.png]]




```
picoCTF{s3cur3_c0nn3ct10n_65a7a106}
```

## Referencias

- [ssh(1): OpenSSH SSH client - Linux man page](https://linux.die.net/man/1/ssh) 
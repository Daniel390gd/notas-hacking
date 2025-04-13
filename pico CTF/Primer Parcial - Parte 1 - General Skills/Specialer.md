
## Descripción 

Reception of Special has been cool to say the least. That's why we made an exclusive version of Special, called Secure Comprehensive Interface for Affecting Linux Empirically Rad, or just 'Specialer'. With Specialer, we really tried to remove the distractions from using a shell. Yes, we took out spell checker because of everybody's complaining. But we think you will be excited about our new, reduced feature set for keeping you focused on what needs it the most. Please start an instance to test your very own copy of Specialer.`ssh -p 61511 ctf-player@saturn.picoctf.net`. The password is `d137d16e`
### pista

What programs do you have access to?
## Solución

- Nos conectamos al servidor con el comando ssh.
- Usando el tabulador vemos que comandos se pueden usar.
- Usando echo podemos listar archivos.
![[10-Specialer_IMG1.png]]
- Usando echo podemos leer los archivos, leyendo uno llamado cala/kazam.txt que tiene la bandera.
![[10-Specialer_IMG2.png]]



```
picoCTF{y0u_d0n7_4ppr3c1473_wh47_w3r3_d01ng_h3r3_838b49d1}
```

## Referencias

- https://youtu.be/OR-DNz5dksY?si=Wuvvaw_kq5eTLZ5v
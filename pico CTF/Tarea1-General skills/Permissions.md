
## Descripción 

Can you read files in the root file?The system admin has provisioned an account for you on the main server:`ssh -p 61488 picoplayer@saturn.picoctf.net`Password: `j4ks-9nxB-`Can you login and read the root file?
### pista

- What permissions do you have?
## Solución

- Nos conectamos al servidor con los datos dados en la descripción.
- Dentro vemos que si usamos el comando ls no sale nada, por lo que usando ls -la podemos ver los archivos y sus permisos
- Usamos cd .. hasta encontrar root
![[01-Permissions_IMG1.png]]
- Intentamos entrar a root con la contraseña.
![[01-Permissions_IMG2.png]]
- Usamos el comando que viene en gtfobins y vemos que ya somos root.
![[01-Permissions_IMG3.png]]
- Seguimos usando ls -la hasta que vemos que existe un archivo con la bandera.
- Usamos cat para obtener la bandera.
![[01-Permissions_IMG4.png]]



```
picoCTF{uS1ng_v1m_3dit0r_021d10ab}
```

## Referencias

- https://youtu.be/ZCM8pLNE2TE?si=t0WPBRcSSAAEA9FY
- [vi | GTFOBins](https://gtfobins.github.io/gtfobins/vi/)
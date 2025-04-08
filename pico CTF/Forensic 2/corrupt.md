
## Descripción 

We found this [file](https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/mystery). Recover the flag.
### pista

Try fixing the file header
## Solución

- Con el comando wget descargamos el archivo "mistery"
![[03-c0rrupt_IMG1.png]]
-  Usando los comandos files y xxd vemos que se puede tratar de un archivo png que podría estar dañado.
- Cambiamos con un editor hexadecimal los bytes de la cabecera 
![[03-c0rrupt_IMG2.png]]

- Vemos que aun no reconoce el archivo como png por lo que checando vemos que no existe un chunk critico llamado IMDHR, por lo que volveremos al editor para cambiar eso.
![[03-c0rrupt_IMG3.png]]
- Ya con eso lo reconoce como archivo png pero el editor eog no lo abre, por lo que instalaremos pngcheck.
![[03-c0rrupt_IMG4.png]]
- Con esta herramienta instalada veremos donde tenemos el error, que es en el chunk PHYS.
![[03-c0rrupt_IMG5.png]]
- Volvemos al editor hexadecimal para corregir.
![[03-c0rrupt_IMG6.png]]
- Ahora el error esta en el chunk IDAT, por lo que volvemos a corregir en el editor.
![[03-c0rrupt_IMG7.png]]
- Usando pngcheck vemos que no hay errores y ahora usando eog vemos la imagen.
![[03-c0rrupt_IMG8.png]]

![[03-c0rrupt_IMG9.png]]




```
picoCTF{c0rrupt10n_1847995}
```

## Referencias

- https://youtu.be/7zY4VkiWbBI?si=62rFbcnq7fnacjC4
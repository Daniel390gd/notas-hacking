
## Descripción 

Alright, enough of using my own encryption. Flask session cookies should be plenty secure! [server.py](https://mercury.picoctf.net/static/60f76192f6e1fea6f4e6e8c5fc9a6a27/server.py) [http://mercury.picoctf.net:44693/](http://mercury.picoctf.net:44693/)
### pista

How secure is a flask cookie?
## Solución

- Entramos en la pagina dada por la descripción.
- Si vemos la cookie esta codificada, si la decodificamos es el valor de la galleta que pusimos.
- Observamos el codigo del archivo server.py, para esto usaremos el comando wget.
![[04-Most-Cookies_IMG1.png]]
- Del código tomaremos los nombres de las galletas.
![[04-Most-Cookies_IMG2.png]]
- Haremos un archivo con el nombre de las galletas.
- Usaremos flask unsign para ejecutar un ataque de fuerza bruta, primero instalaremos la herramienta con el comando sudo apt install.
- Como hubo problemas al instalarlo vamos a crear un ambiente virtual, para evitar problemas.![[04-Most-Cookies_IMG3.png]]
![[04-Most-Cookies_IMG4.png]]

- Una vez instalado el ambiente usaremos pip para instalar la herramienta.
![[04-Most-Cookies_IMG5.png]]
- Instalada usamos la herramienta para obtener la cookie.
![[04-Most-Cookies_IMG6.png]]
- Ahora usamos sign para forjar la cookie codificada y una vez que la tenemos usamos curl para obtener la bandera.
![[04-Most-Cookies_IMG7.png]]



```
picoCTF{pwn_4ll_th3_cook1E5_dbfe90bf}
```

## Referencias

- https://youtu.be/ufs1xqSQCUM?si=DPwfBd5gEi4mtFYl
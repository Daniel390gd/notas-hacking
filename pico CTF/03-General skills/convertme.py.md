
## Descripción 

Run the Python script and convert the given number from decimal to binary to get the flag.[Download Python script](https://artifacts.picoctf.net/c/24/convertme.py)
### pista

- Look up a decimal to binary number conversion app on the web or use your computer's calculator!
- The `str_xor` function does not need to be reverse engineered for this challenge.
- If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.
- To use `wget` in the webshell, first right click on the download link and select 'Copy Link' or 'Copy Link Address'
- Type everything after the dollar sign in the webshell: `$ wget` , then paste the link after the space after `wget` and press enter. This will download the script for you in the webshell so you can run it!
- Finally, to run the script, type everything after the dollar sign and then press enter: `$ python3 convertme.py`
## Solución

- Usamos el comando wget para descargar el archivo convertme.py
![[04-convertme.py_IMG1.png]]
- Usando python3 y nombre del archivo lo ejecutamos en la terminal.
- Usando ciberchef convertimos el 79 a binario, con esto obtendremos la bandera.
![[04-convertme.py_IMG2.png]]



```
picoCTF{4ll_y0ur_b4535_722f6b39}
```

## Referencias

- [CyberChef](https://cyberchef.org/)
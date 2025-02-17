## Descripción 

Our flag printing service has started glitching!`$ nc saturn.picoctf.net 59227`

### pistas

- ASCII is one of the most common encodings used in programming
- We know that the glitch output is valid Python, somehow!
- Press Ctrl and c on your keyboard to close your connection and return to the command prompt.

## Solución

1. Ejecutamos en el web Shell el servicio nc saturn.picoctf.net 50481 el puerto nunca sera el mismo.

![[09-Glitch_Cat_IMG1.png]]

2. Ejecutamos con el interprete de python la cadena que nos da el paso anterior.

![[09_Glitch_Cat_IMG2.png]]

```
picoCTF{gl17ch_m3_n07_bda68f75}
```

## Notas adicionales

- 
## Referencias

- [picoCTF - picoGym Challenges]
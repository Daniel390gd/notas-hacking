
## Descripción 

Theres tapping coming in from the wires. What's it saying `nc jupiter.challenges.picoctf.org 48247`.
### pista

- What kind of encoding uses dashes and dots?
- The flag is in the format PICOCTF{}
## Solución

- Ingresamos con el comando nc al servidor y vemos que nos da lo siguiente:
![[06-Tapping_IMG1.png]]
- Investigando lo que nos dice la primera pista vemos que lo que nos dieron es un codigo morse.
![[06-Tapping_IMG2.png]]
- Usamos un traductor de codigo morse y obtenemos la bandera
![[06-Tapping_IMG3.png]]



```
picoCTF{M0RS3C0D31SFUN1261438181}
```

## Notas adicionales

Hay que colocar la bandera con el formato picoCTF{}
## Referencias

- [Traductor de código morse](https://morsecodetranslator.com/es/)
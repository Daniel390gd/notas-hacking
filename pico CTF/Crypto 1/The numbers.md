
## Descripción 

The [numbers](https://jupiter.challenges.picoctf.org/static/f209a32253affb6f547a585649ba4fda/the_numbers.png)... what do they mean?
### pista

The flag is in the format PICOCTF{}
## Solución

- Con wget descargamos la imagen.
- Al abrir la imagen vemos varios numeros con el formato de la bandera, pues estan las llaves.
![[01-The-numbers_IMG1.png]]
- Investigando la bandera esta cifrada en A1Z26(donde cada numero es una letra del alfabeto, ejemplo A = 1 y Z =26), por lo que usando ciyberchef desciframos y obtenemos la bandera.
![[01-The-numbers_IMG2.png]]



```
picoCTF{thenumbersmason}
```


## Descripción 

Decode this [message](https://jupiter.challenges.picoctf.org/static/d6fcea5e3c6433680ea4f914e24fab61/message.wav) from the moon.
### pista

- How did pictures from the moon landing get sent back to Earth?
- What is the CMU mascot?, that might help select a RX option

## Solución

- Con el comando wget descargamos el mensaje.
![[01-m00nwalk_IMG1.png]]
- No vamos a la carpteta "otp" y clonamos el repositorio de git con la herramienta Scottie.
![[01-m00nwalk_IMG2.png]]
- Una vez clonado el repo nos metemos a la carpeta "sstv" y ejecutamos el script de instalación.
![[01-m00nwalk_IMG3.png]]
- Una vez instalada la herramienta ejecutamos el siguiente comando: "sstv -d message.wav -o result.png"
![[01-m00nwalk_IMG4.png]]
- Abrimos el archivo resultado.png que contiene la bandera, cuando abrimos esta esta al reves por lo que tendremos que rotar la imagen.
![[01-m00nwalk_IMG5.png]]




```
picoCTF{beep_boop_im_in_space}
```

## Referencias

- https://youtu.be/UyLTEpAz6eE?si=l97e8IqVEADh-Nqx
- [colaclanth/sstv: SSTV Decoder](https://github.com/colaclanth/sstv)
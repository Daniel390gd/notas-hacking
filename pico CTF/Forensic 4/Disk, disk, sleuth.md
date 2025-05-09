
## Descripción 

Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag in this disk image: [dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/a734f18939e0aaea9d27bc7a243a0ed0/dds1-alpine.flag.img.gz)
### pista

- Have you ever used `file` to determine what a file was?
- Relevant terminal-fu in picoGym: https://play.picoctf.org/practice/challenge/85
- Mastering this terminal-fu would enable you to find the flag in a single command: https://play.picoctf.org/practice/challenge/48
- Using your own computer, you could use qemu to boot from this disk!

## Solución

- Descargamos la imagen de disco con wget.
![[02-Disk-disk-sleuth_IMG1.png]]
- Desempaquetamos la imagen con gzip.
![[02-Disk-disk-sleuth_IMG2.png]]
- Usamos el comando srch_strings para obtener la bandera.
![[02-Disk-disk-sleuth_IMG3.png]]




```
picoCTF{f0r3ns1c4t0r_n30phyt3_a69a712c}
```

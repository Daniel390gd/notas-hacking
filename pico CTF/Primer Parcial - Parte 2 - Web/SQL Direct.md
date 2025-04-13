
## Descripción 

Connect to this PostgreSQL server and find the flag!`psql -h saturn.picoctf.net -p 56081 -U postgres pico`Password is `postgres`
### pista

What does a SQL database contain?
## Solución

- Nos conectamos al servidor.
![[Pasted image 20250412193417.png]]
- Usando help ejecutamos \d para ver las tablas y vemos que existe una llamada flag.
![[Pasted image 20250412193510.png]]
- usamos table flags; para ver su contenido y ahí esta la bandera.
![[Pasted image 20250412193520.png]]



```
picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}
```

## Referencias

- https://youtu.be/iK68Xr3sNPQ?si=Nl0nnd5d3JSxQ6Hb
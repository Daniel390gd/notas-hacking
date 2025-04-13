
## Descripción 

Connect to this PostgreSQL server and find the flag!`psql -h saturn.picoctf.net -p 56081 -U postgres pico`Password is `postgres`
### pista

What does a SQL database contain?
## Solución

- Nos conectamos al servidor.
![[08-SQL-Direct_IMG1.png]]
- Usando help ejecutamos \d para ver las tablas y vemos que existe una llamada flag.
![[08-SQL-Direct_IMG2.png]]
- usamos table flags; para ver su contenido y ahí esta la bandera.
![[08-SQL-Direct_IMG3.png]]



```
picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}
```

## Referencias

- https://youtu.be/iK68Xr3sNPQ?si=Nl0nnd5d3JSxQ6Hb
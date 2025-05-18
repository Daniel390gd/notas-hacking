
## Descripción 

Class, take your seats! It's PRIME-time for a quiz... `nc jupiter.challenges.picoctf.org 1981`
### pista

[RSA info](https://simple.wikipedia.org/wiki/RSA_algorithm)
## Solución

- Nos conectamos con nc.
- Nos hace una pregunta, para responderla basta con multiplicar "p" y "q".
![[rsa-pop-quiz_IMG1.png]]
- La siguiente pregunta es similar pero en este caso haremos un despeje, para obtener q a "n" lo dividimos entre "p".
![[rsa-pop-quiz_IMG2.png]]
- La tercera pregunta no nos dan suficientes datos para responderla por lo que ponemos N.
- La cuarta pregunta es solamente usar la formula del totient.
![[rsa-pop-quiz_IMG3.png]]
- Para la  quinta pregunta usamos la formula del texto cifrado(c).
![[rsa-pop-quiz_IMG4.png]]
- Para la sexta pregunta igual que la tercera no nos dan suficiente información, por lo que no se puede responder.
- Para la septima debemos obtener la llave privada(d), primero obtenemos el totient(n) con los datos que nos dan y luego usando la función inverse lo calculamos.
![[rsa-pop-quiz_IMG5.png]]
- Para la ultima pregunta empezamos obtiendo q que ya sabemos como obtener si se tiene "p" y "n", posteriormente calculamos totient(n) y con este calculamos la llave privada, ya con la llave privada usamos pow para obtener el texto descifrado(m), una vez que lo tenemos usamos la función long_to_bytes y obtenemos la bandera.
![[rsa-pop-quiz_IMG6.png]]



```
picoCTF{wA8_th4t$_ill3aGal..ode01e4bb}
```

## Notas adicionales

c - texto cifrado
m - mensaje en texto plano
p - número primo 1
q - número primo 2
n - modulo -> n = p *q*
tn - titien n -> tn = (p-1)*(q-1)*
e - exponente (llave publica) -> (2^16+1) = 65537
d - Llave privada -> d = e mod inv tn / inverse(e,tn)

Para encriptar

c = m^e mod n  / pow(m,e,n) 

Para desencriptar

m = c^d mod n / pow(c,d,n) s
## Referencias

- https://youtu.be/HIwgWauz-fc?si=jihMmp52qp7CbKbm
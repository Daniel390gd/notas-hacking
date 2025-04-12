
## Descripción 

Cookie Monster has hidden his top-secret cookie recipe somewhere on his website. As an aspiring cookie detective, your mission is to uncover this delectable secret. Can you outsmart Cookie Monster and find the hidden recipe?You can access the Cookie Monster [here](http://verbal-sleep.picoctf.net:60118/) and good luck
### pista

- Sometimes, the most important information is hidden in plain sight. Have you checked all parts of the webpage?
- Cookies aren't just for eating - they're also used in web technologies!
- Web browsers often have tools that can help you inspect various aspects of a webpage, including things you can't see directly.
## Solución

- Ingresamos a la pagina dada en la descripción.
![[Pasted image 20250412075609.png]]
- Intentamos acceder con admin como usuario y contraseña pero nos lanza una pista.
![[Pasted image 20250412080044.png]]
- Con esto regresamos al login y inspeccionamos las cookies.
![[Pasted image 20250412075835.png]]
- El valor de la cookie esta codificado en base 64 y contiene caracteres de escape URL, por lo que en ciberchef, usamos la receta URL Decode.
![[Pasted image 20250412075846.png]]
- Una vez hecho esto tomamos la salida y usamos la receta From Base64 y obtenemos la bandera.
![[Pasted image 20250412075942.png]]




```
picoCTF{c00k1e_m0nster_l0ves_c00kies_A964A134}
```

## Referencias

- [CyberChef](https://cyberchef.org/)
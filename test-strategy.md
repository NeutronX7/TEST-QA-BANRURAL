Vulnerabilidades:
- Pude percatarme que en la caja de texto se podían digitar cualquier tipo de caracteres
- Se debe utilizar JQuery para eivtar manipulaciones de valores
- Hacer las peticiones tokenizadas para evitar inyecciones

Correcciones:
- Ahora se ingresan solo caracteres numéricos
- solo se aceptan valores en el rango de 1-100
- los intentos no pasan más de diez veces

Errores encontrados:
- La caja de texto aceptaba todo tipo de caracteres
- No se estaban imprimiendo los resultados

Funcionalidad del código:
- Se utilizó Math.floor para redondear los números de Math.random()
- Se definió el rango de Math.random() para que esté en el rango solicitado con este fragmento de código:
let randomNumber = Math.floor(Math.random() * 100) + 1;
- Se cambió el valor de la variable ATTEMPS  a 10, anteriormente tenía 5
- Se agregó doble signo en vez de triple en las validaciones
- Al reiniciarse el juego siempre tenía el valor de 1, y ahora es un número random
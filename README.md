# Koans

![](https://i.imgur.com/9Ug9NBn.png)

[Koans](https://en.wikipedia.org/wiki/K%C5%8Dan) (公案), son paradojas del budismo zen para probar el avance de los estudiantes en su camino a la iluminación. Están diseñados para hacer pensar o dudar a los estudiantes.

Son, por tanto, aserciones que se deben resolver para entender como funcionan los lenguajes de programación.

Los Koans van incrementando en dificultad conforme avanzas, así que no te desanimes.

## Mecanismo

- Hay una declaración que no pasa un **test**.
- Necesitas cambiar/añadir código para pasar el **test**.

Usaremos Jasmine para realizar los tests.

Abre el navegador y ejecuta el fichero `SpecRunner.html`.

Al principio todos los tests aparecen en amarillo porque están comentados, excepto uno que lanza un error.

Todos los tests se encuentran en la carpeta `spec`. 

Abre el fichero `koans.js` y descomenta la siguiente línea:

```javascript
it('`var` works as usual, it does not restricts scope', () => {
  if (true) {
    /*You should add your code in here*/
  }
  expect(varX).toBe(true);
});
```

Cuando descomentas la línea y refrescas la página `SpecRunner.html` se ve la siguiente página:

![image](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_0a3269347ff9cf345534607ba27809d2.png)

**El objetivo no es finalizar todos los tests. Lo que se pretende es que comprendas por qué falla cada test y cómo lo resuelve javaScript.**

Esta manera de trabajar se denomina Test Driven Development([TDD](https://en.wikipedia.org/wiki/Test-driven_development)):

- Descomenta el test
- Refresca la página
- Cambia el código y pasa el test
- Refresca la página y comprueba si has pasado el test

ℹ️ 
Las líneas de expect no se deben alterar.



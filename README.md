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

When we uncomment the line and refresh the `SpecRunner.html` page, we will see something like that:

![image](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_0a3269347ff9cf345534607ba27809d2.png)

**The primary goal is not to finish all the tests. We want you to understand why each test is failing and how does JavaScript ES6 work in specific scopes.**

To do that, the correct workflow is the one used on Test Driven Development([TDD](https://en.wikipedia.org/wiki/Test-driven_development)):

- Uncomment the test
- Refresh the page to see that the uncommented test is failing
- Change the code to pass the test
- Refresh the page to see that the test is passing

:::warning 
Leave the expect lines unchanged! 👀 
:::

This process has to be done for each test. **Do not uncomment all the tests and launch the app. It will be more difficult for you to see if your code is passing the tests.**

Since the Koans includes tests about a lot of the ES6 features, you can keep practicing individually after class. 

As we said, this is an excellent way to learn things about a programming language. 

Happy coding! :heart:

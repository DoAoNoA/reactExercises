 
## CLASE 0505  :octocat:   
**_ES6 fundamentals_**


:clock1: **_let:_**  Variable no es tipo de dato. 
 **_const:_**  No cambia.

:clock2: [import / export:](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Sentencias/export)

* Export con nombre: 
  * Son útiles cuando se necesitan exportar múltiples valores. 
  * Durante el import, es obligatorio usar el mismo nombre que el correspondiente objeto.
  
    > En el módulo, podremos usar el siguiente código:
    ```javascript
      // module "my-module.js"
      function cube(x) {
        return x * x * x;
      }
      const foo = Math.PI + Math.SQRT2;
      export { cube, foo };
    ```   
    
    > De esta forma, en otro script , podemos tener:
    ```javascript
      import { cube, foo } from 'my-module';
      console.log(cube(3)); // 27
      console.log(foo);    // 4.555806215962888
    ```   
  
* Export por defecto:
  Puede ser importado con cualquier nombre.
  * Solo puede haber un export por defecto.
    ```javascript
      export default k = 12; // en el archivo test.js 

      import m from './test' 
      // notese que tenemos la libertad de usar import m en lugar de import k, porque
      // k era el export por defecto 
      console.log(m); // escribirá 12




:clock3: arrow functions


default arguments
template strings
spread operator array
spread operator object
destructuring
...rest
classes
promises
async await
Object.keys, Object.values
map, filter and reduce

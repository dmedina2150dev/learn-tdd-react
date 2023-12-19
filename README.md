# Testing TDD (Test Driven Development)

Es una tecnica de desarrollo que se enfoca en crear los test antes del codigo de produccion

Se basa en tomar los requerimientos o casos de uso al desarrollar una aplicación. Recrear estos requerimientos por medio de pruebas, posteriormente pasar estas pruebas al codigo de la funcionalidad.

El Flujo de TDD:
 - (RED) Crear un test que falle, significa que en principio al crear el test este debe fallar.
 - (GREEN) Desarrollar la funcionalidad que cumpla el test y esta vez el test si pase o no falle. Es importante desarrollar lo minimo necesario para que el Test pase.
 - (ORANGE) En esta face detectamos codigo que se pueda mejorar, y solventar malas practicas. Y realizamos el refactor del codigo.

# Jest

Caracteristicas:
> Es un framework de testing para Javascript.

- __Creado por Facebook__ - Actualmente es mantenido por facebook y por la comunidad
- __Javscript Testing Framework__ (Es agnostico al framework)
- __Zero configuration__ - Uno de los pilares de Jest es que no posea tantas configuraciones y sea facil de usar. Esto no significa que no pueda personalizarlo y configurarlo.
- __Snapshots__ - Significa que nos brinda la estructura de un componente en cierto momento.
- __Isolated__ - Nos permite ejecutar los test de forma independientes unos de otros y tambien de forma paralela.
- __Code Coverage__ Información que nos provee Jest, sin la necesidad de instalar otras dependencias. Con una bandera especial (--coverage) sobre que lineas de nuestro codigo esta siendo cubiertas por el Test.
- __Easy Mocking__ Es posible crear Objetos Mock, que son una manera de reemplazar una implementación con un objeto replica fake.




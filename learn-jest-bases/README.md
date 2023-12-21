# Aprender base de Jest

Configuración inicial de Jest

**NOTA:** Ciertas configuraciones pueden fallar en principio, se debe ir evaluando que es lo que esta fallado.

1. Instalar Jest [Guia Oficial](https://jestjs.io/es-ES/docs/getting-started)
```
npm install --save-dev jest
```
2. Crear Script en el __package.json__
```
{
  "scripts": {
    "test": "jest"
  }
}
```
3. Crear el archivo de configuraciones automatico con el comando: 
```
npm init jest@latest
```
**NOTA:** Esto creara el __jest.config.js__ con las configuraciones que vayas indicando al ejecutar el comando anterior, se pueden ir modificando a las necesidades del proyecto

4. En este caso estamos usando babel como se puede ver al final de este documento para el fast reload. Debemos agregar las dependencias:
```
npm install --save-dev babel-jest @babel/core @babel/preset-env
```

5. Ahora creamos el archivo __babel.config.cjs__
**NOTA:** En este caso el archivo tiene como extensión __cjs__ indicando que es compatible con commonJS para evitar ciertos errores que se pueden observar al cambiar la extención a __js__ 

Contenido inicial del archivo:

```javascript
module.exports = {
  presets: [['@babel/preset-env', {targets: {node: 'current'}}]],
};
```

6. 



# Aplicación de React + Vite

Esta plantilla proporciona una configuración mínima para que React funcione en Vite con HMR y algunas reglas de ESLint.

Actualmente, hay dos complementos oficiales disponibles:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) usa [Babel](https://babeljs.io/) para actualización rápida
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) usa [SWC](https://swc.rs/) para actualización rápida

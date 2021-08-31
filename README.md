# [Proyecto Frecuencia de Palabras y Proceso *.txt en Mongo]

**El proyecto** esta basado en codigo python, utilizando diversas librerias y en el framework Flask .

Se utilizó el framework de **[Bootstrap](https://getbootstrap.com/)** para el uso amigable de las URLs.

El proyecto consta de varias URLS a mencionar:
- / (home o root): acceso al home del sitio
- /importtxt: pre-proceso de importacion de archivos de text (extension .txt)
- /api/docs/: API para contar la frecuencia de 1 palabra de acuerdo a los parametro.
- /login: URL para autenticacion, genera un token para la sesión.

Cabe mencionar que la interface /api/docs maneja 2 parametros:
```bash
term = debe tener como valor una palabra o numero a buscar ( no debe incluir espacios)
doc_name = nombre del documento donde se desea buscar/contar la palabra. El nombre ingresado puede o no incluir la extension .txt al final del parametro.
```
Ejemplo: http://127.0.0.1:5000/api/docs?term=pero&doc_name=10825-8.txt

```bash
{
  "texto": [
    "10825-8.txt", 
    "pero", 
    87
  ]
}
```
## Instalación
A continuacion describimos los pasos de instalación.

### Instalación de librerias
mediante el comando pip, deben instalarse las librerias Python:

1. `npm install` (install npm deps)
2. _Optional:_ `npm run dev` (developer mode, autocompile with browsersync support for live demo)
3. `npm run production` (compile css/js files)

## Librerias utilizadas
Lista de frameworks, librarias Python utilizado:
- [Database Drivers](#database-drivers)

## Database
*Librarias para conectar y gestionar bases de datos.*
* NoSQL Databases
	* [pymongo](https://github.com/mongodb/mongo-python-driver) - Cliente Python oficial para MongoDB.

## Framework
*Librarias para la gestion del framework.*

### Comando para implementar
#### Git
```bash
git clone https://github.com/cadupar20/melidocs.git
```
## Browsers soportados

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br/>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br/>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br/>Chrome 
| --------- | --------- | --------- |
| last version Edge| last version| last version| 

## Licencia

Este proyecto es open source, puede ser utilizado y compartido libremente.

## Referencias
- [Python](http://www.pixeden.com/psd-web-elements/flat-responsive-showcase-psd)
- [Flask](https://www.graphicsfuel.com/2013/02/13-high-resolution-blur-backgrounds/)
- [Pymongo](https://pickaface.net/)

# Proyecto Final Sprint 2 

Los estudiantes basados en el sitio web construido durante la sesión 4 en donde se actualizó utilizando VUE, el sitio web desarrollado en la sesión 1; deberán hacer uso de loscomponentes reutilizables de VUE y de las APIs explicadas durante la sesión 3. El sitio web resultante deberá contar con las secciones de encabezado, en donde estará el menú y el banner, una sección intermedia que presentará, en el mismo formato de las 4 noticias en dos filas y 2 columnas, el uso de una API a elección de los estudiantes,recomendamos una API de noticias como Colombia news API o la API de películas vista durante la sesión 3.

-Se debe contar con una sección para los integrantes que consumirá la información de los miembros desde un JSON tal como se explicó en la sesión 4. Como ejemplo del resultado esperado durante la sesión se mostrará el sitio web funcionando con los componentes base necesarios. Para esto deberá construir un componente reutilizable.

-Componente 1 (Tarjeta de miembro): El componente se debe llamar TeamCard y debe estar en la carpeta de components. Donde acepta el objeto member que es el miembro      del equipo el objeto debe de ser de la siguiente forma:

```
{
  codigo: 1,
  nombre: 'Lucas Mera',
  descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscingelit. Mauris condimentum ac elit et accumsan.',
  rol: 'Desarrollador backend',
  image: 'path/to/image'
}
```

-La tarjeta debe mostrar la imagen del miembro. Y debe de mostrar en el body de la tarjeta la información de código, rol, nombre y descripción.
 
## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your unit tests
```
npm run test:unit
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

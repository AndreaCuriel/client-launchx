# vue-3-crud

El repositorio contiene un Cliente en Vue, que muestra una lista de Explorers por su username, la cual puede visualizar toda la información al darle clic a cada uno.
Permite la actualizacion de información, la eliminación y la creacion de un nuevo Explorer.

Para su funcionamiento es necesario el servidor y una Base de Datos. Puedes encontrar [aquí](https://github.com/AndreaCuriel/API-Express-DB) el servidor.

## Correr la aplicacion Cliente Servidor.
1. Realiza un fork y clona los repositorios del Cliente y del servidor e instala las dependencias necesarias con `npm intall`.
2. Verificar que los URLs del Servidor y del Cliente esten correctas en los siguientes archivos.
- Servidor: En el archivo server.js en la línea 13, donde es la inicialización del CORS, la URL es: `"http://localhost:8081"` (Url donde corre el Cliente, puede variar la url, en su caso verificar cual es la correspondiente). [server.js](https://github.com/AndreaCuriel/API-Express-DB/blob/main/server.js)
- Cliente: En el archivo `http-common.js` en la carpeta src, la cual contienela configuración de Axios. En la línea 3 verifica la url `localhost:3000` (ulr donde corre el Servidor). [Código](https://github.com/AndreaCuriel/client-MC/blob/master/src/http-common.js)
3. Servidor: Ingresar la información de la Base de Datos para tener una exitosa conexion con la API. La cual se encuentra en `.env`. No versione el username y password. [.env](https://github.com/AndreaCuriel/API-Express-DB/blob/main/.env)
4. Servidor: Corre la app con `node server.js`.
5. Cliente: Corre la app con `npm run serve`.


## Diagrama del Cliente en VUE.

![diagramaClienteVue](https://user-images.githubusercontent.com/99285898/167320099-0905c3cd-b321-413a-9d90-f515fd687457.png)

## Visualización de la App (http://localhost:8081/)

![cliente](https://user-images.githubusercontent.com/99285898/167320679-c9751b69-4e51-4316-a8f0-fa3a2bd73d57.png)













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

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

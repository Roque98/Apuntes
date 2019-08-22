# Conectar con mongo

> Referencia
> [Pagina de mongoose](https://www.npmjs.com/package/mongoose)

## Paso 1

- Instalar la libreria

```
npm i mongoose
```

## Paso 2 

- importar la libreria

```JAVASCRIPT
const mongoose = require('mongoose');
```

## Paso 4

- Levantar mongod

```
$> mongod
```

## Paso 5

- conectar con la base de datos
- No olvidar

```JAVASCRIPT
// Rutas
// ...

//Base de datos
mongoose.connect('mongodb://localhost:27017/my_database', { useNewUrlParser: true }, (err, res) => {
    if (err) throw err;

    console.log('base de datos ONLINE');

});


//Iniciar server
// ...
```

## Codigo completo de server.js

```JAVASCRIPT
const express = require('express');
const mongoose = require('mongoose');


const app = express();

require('./config/config');

// Rutas 
app.use(require('./routes/usuario.js'));

//Base de datos
mongoose.connect('mongodb://localhost:27017/my_database', { useNewUrlParser: true }, (err, res) => {
    if (err) throw err;

    console.log('base de datos ONLINE');

});

// Iniciar servidor
app.listen(process.env.PORT, () => {
    console.log('Escuchando el puerto ', process.env.PORT);
})
```

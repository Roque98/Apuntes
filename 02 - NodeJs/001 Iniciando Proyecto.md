# Primeros pasos

## Objetivo

> Iniciar un servidor en node

### Paso 1

    npm init

- presionar npm init
- despues varios enters para llenar informacion

> Esto creara el el package.json

### Paso 2

Instalar express

    npm i express

### Paso 3

- crear el directorio **server/server.js**

### Paso 4

- Crear un server hola mundo

```javaScript
const express = require('express')
const app = express()

app.get('/', function(req, res) {
    res.json({
        ok: true,
        message: 'Hola mundo Node'
    })
})

app.listen(3000, () => {
    console.log('Escuchando el puerto 3000');
})
```

### Paso 5

Iniciar servidor

    nodemon server/server

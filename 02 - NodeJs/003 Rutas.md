# Rutas servidor

## Paso 1

Instalar body parser

> Body parser nos permite obtener los datos que se envian desde el frontend de forma muy sencilla

    npm i body-parser

## Paso 2

Crear archivo 

> server/routes/usuario.js

## Paso 3

Contenido server/routes/usuario.js

```JAVASCRIPT
const express = require('express')
const app = express()

// ********** CRUD Create, Read, Update, Delete ***********

// =====================
// Create - post Usuario
// =====================
app.post('/usuario', function(req, res) {
    res.json({
        ok: true,
        message: 'post Usuario - Listo'
    })
})


// =====================
// Read - Get Usuario
// =====================
app.get('/usuario', function(req, res) {
    res.json({
        ok: true,
        message: 'Get Usuarioe'
    })
})

// =====================
// Update - Put 
// =====================
app.put('/usuario', function(req, res) {
    res.json({
        ok: true,
        message: 'Put Usuario - Listo'
    })
})

app.put('/usuario/:id', function(req, res) {

    let id = req.params.id;

    res.json({
        ok: true,
        message: 'Put Usuario - Listo',
        id
    })
})

// =====================
// Delete - delete Usuarrio
// =====================
app.delete('/usuario', function(req, res) {
    res.json({
        ok: true,
        message: 'Delete usuario listo'
    })
})



module.exports = app;
```

## Paso 4

Usar rutas en el index

```JAVASCRIPT
// Rutas
app.use(require('./routes/usuario.js'));
```
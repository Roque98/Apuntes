# config.js

## Paso 1

Crear archivo

> server / config / config.js

```java
// =====================
// Puerto
// =====================
process.env.PORT = process.env.PORT || 3000;
```

## Paso 2

Configurar el archivo server/server.js

```JAVASCRIPT
const express = require('express')
const app = express()
require('./config/config');

app.get('/', function(req, res) {
    res.json({
        ok: true,
        message: 'Hola mundo Node'
    })
})

app.listen(process.env.PORT, () => {
    console.log('Escuchando el puerto ', process.env.PORT);
})
```

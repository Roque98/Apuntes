# Seccion 4

## Definiciones

### Definiciones de  un archivo

Muestra el nombre de todo lo que se ha declarado en el archivo

    ctrl + p escribir @

### Cambiar el nombre de las variables o el nombre de las clases

    F2

## Buscar

### Ir a la linea

Puedes ir directamente a la linea de codigo que tu quieras

    ctr + g

### Buscar y remplazar

    ctrl + h

## Crear snipet

> Archivo > preferencias > fragmentos de codigo del usuario

- Bucar el nombre del lenguaje al que se quiera integrar el sniper

```
"Crear una clase": {
        "prefix": "clase",
        "body": [
            "export class ${1:NombreClase} {",
            "",
            "   construtor($2) {",
            "       $3",
            "   }",
            "}"
        ],
        "description": "Crea la estrcutura basica de una clase de typeScript"
}
```

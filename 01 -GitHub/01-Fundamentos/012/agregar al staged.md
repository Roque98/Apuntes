# Formas de agreagar archivos al staged

Agregar solo un archivo

    git add NOMBRE_ARCHIVO.png

Agregar una lista de archivos

    git add NOMBRE_ARCHIVO.png NOMBRE_ARCHIVO2.HTML

Agregar todos los archivos 

    git add --all 

Agrega todo los .png del proyecto enterto

    git add "*.png"

Agrega todo los .png del directorio actual

    git add *.png

Todo lo de una  carpeta

    git add css/

Escluir algo del staged

    git reset NOMBRE_ARCHIVO.*

# Viajes en el tiempo

## Arreglar errores del futuro

> Estos comandos permiten regresar a un punto en el tiempo y revertir los cambios
> hechos

## Regresar a ese punto en el tiempo

    git reset --soft idCortoCommit

> Soft =>

"elimina" los commits posteriores al commit al que estas haciendo el reset
conserva los cambios en el stage area
conserva los cambios que tengas en tus archivos (working directory)

> Mixed =>

"elimina" los commits posteriores al commit al que estas haciendo el reset
Deshace los cambios en el stage area
conserva los cambios que tengas en tus archivos (working directory)

> Hard =>

"elimina" los commits posteriores al commit al que estas haciendo el reset
Deshace los cambios en el stage area
Deshace los cambios que tengas en tus archivos (working directory)

## Registro historico de git

    git reflog

## Recuperar de los viajes en el tiempo

    git reset --hard [idCommit]

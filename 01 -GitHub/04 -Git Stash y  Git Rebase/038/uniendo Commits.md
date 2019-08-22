# Uniendo commits

si quisiesemos unir los ultimos 2 commits en uno solo

![img1]

## usando git interactivo

    git rebase -i HEAD~4

> - i: indica que sera un rebase interactivo
> - HEAD~4 : en el editor tomara los ultimos 4 commits

Ejemplo: 

![img2]

## aplicando un squash

> Esto especifica que queremos unificar commits en uno solo

Ejemplo:

![img3]

## Agregar un commit que guarde la combinacion de los commits

Ejemplo:

![img4]

## Resultado final

![img5]

<!-- Declaracion de imagenes -->

[img1]: img/01.jpg
[img2]: img/02.jpg
[img3]: img/03.jpg
[img4]: img/04.jpg
[img5]: img/05.jpg


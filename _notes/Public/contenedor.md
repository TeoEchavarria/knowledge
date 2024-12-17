---
title: Contenedor
feed: show
date: 09-12-2024
tags:
  - devOps
  - docker
curso:
---
Medio para empaquetar una aplicacion con todas las dependencias
## Principales caracteristicas
- **Portables:** Facil de compartir entre desarrolladores y operaciones
- **Dinámico**: Mientras el contenedor está en funcionamiento, puedes interactuar con él, modificar su estado, almacenar datos temporales, etc.
- **Capa de Escritura**: Al crear un contenedor a partir de una imagen, Docker añade una capa de escritura que permite cambios temporales en el contenedor sin alterar la imagen original.
- **Ciclo de Vida**: Los contenedores pueden iniciarse, detenerse, reiniciarse y eliminarse según las necesidades, lo que les da un comportamiento más dinámico comparado con las imágenes.

Es una instancia **en ejecución** de una [[imagen - docker]]. Representa la aplicación funcionando en un entorno aislado.

# Crear un contenedor
```
docker create --name <name-container> <imagen-base>
```

Y luego para correr el contenedor
```
docker run [opciones] <imagen>
```
Y para ver cuales contenedores estan corriendo
```
docker ps -a
```
Y para detener el contenedor
```
docker stop <id_contenedor> | <nombre_contenedor>
```
y para eliminar el contenedor
```
docker rm <id_contenedor> | <nombre_contenedor>
```

>[!note] Relacionado con: [[docker]] [[linux]] [[virtual env]] [[kernel]]


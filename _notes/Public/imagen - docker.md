---
title: Imagen Docker
feed: show
date: 09-12-2024
tags:
  - devOps
  - docker
curso:
---
Una **imagen de [[docker]]** es una plantilla inmutable que contiene todo lo necesario para ejecutar una aplicación. Esto incluye:

- **Sistema Operativo**: Una base sobre la cual se ejecuta la aplicación (por ejemplo, una distribución de [[linux]]).
- **Dependencias**: Librerías, paquetes y herramientas necesarias para que la aplicación funcione correctamente.
- **Código de la Aplicación**: El propio código fuente o binarios de la aplicación que se va a ejecutar.
- **Configuraciones**: Variables de entorno, archivos de configuración y otros ajustes necesarios para la ejecución.
 
### **Características Clave de las Imágenes de Docker**

1. **Inmutabilidad**: Una vez creada, una imagen no cambia. Si se necesita una versión actualizada, se construye una nueva imagen.
2. **Portabilidad**: Las imágenes son consistentes en cualquier entorno que soporte Docker, lo que garantiza que la aplicación se ejecutará de la misma manera en desarrollo, pruebas y producción.
3. **Reutilización**: Gracias al sistema de capas, las imágenes pueden compartir partes comunes, reduciendo el tamaño total y acelerando las descargas.
4. **Versionado**: Las imágenes pueden versionarse mediante etiquetas, lo que facilita el seguimiento de cambios y la gestión de diferentes versiones de una aplicación.
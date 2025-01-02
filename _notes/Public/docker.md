---
title: Docker
feed: show
date: 26-11-2024
tags:
  - devOps
curso:
---
Es una plataforma de contenedores que permite a los desarrolladores empaquetar aplicaciones y sus dependencias en un formato estándar llamado contenedor. Los contenedores de Docker proporcionan un entorno de ejecución completamente aislado, similar a una [[virtual env|máquina virtual]], pero más ligero y más eficiente.

### Docker Images
- Para ver todas las [[imagen - docker]] que has descargado
```
docker images
```

- Para descargar una imagen
```
docker pull <name-image>:<version-image>
```

- Para Eliminar una imagen
```
docker image rm <name-image>:<version-image>

docker rmi <id_imagen> | <nombre_imagen>:<tag>
```

>[!warning] Para agregar docker a [[nix]] lo que se debe de hacer es:
>- De forma temporal 
>```
>nix-shell -p docker
>```
>- De forma permanente con comandos 
>```
>nix-env -iA nixos.docker
>```
>- Dentro de la configuracion 
>```
>  environment.systemPackages = [pkgs.docker];
>```


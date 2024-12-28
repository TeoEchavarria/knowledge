---
title: Formatear USB en Mac
feed: show
date: 28-12-2024
tags: 
curso:
---
Puede hacerse por linea de comandos, de la forma:
```
diskutil list
```

Para ver todos los discos tanto internos como externos
Luego ha alguno que dira algo como: 
```
/dev/disk# (external, physical):
```

Para formatearla hacemos 
```
diskutil unmountDisk /dev/disk#
```


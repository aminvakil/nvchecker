

# nvchecker
Verificador de nuevas versiones para lanzamientos de software

Este repositorio incluye paquetes e imágenes de Docker upstream que utilizo para mantener mis paquetes AUR e imágenes de Docker.

Se ejecuta diariamente para verificar actualizaciones y crea pull requests cuando hay actualizaciones disponibles.

## Ámbito

Este repositorio se mantiene para el seguimiento personal de paquetes e imágenes. No está destinado a ser un registro de paquetes compartido y no se aceptan pull requests que añadan paquetes para otras personas. Si deseas rastrear tus propios paquetes, por favor haz un fork del repositorio y personaliza los archivos `*.toml` y los flujos de trabajo para tu propio uso.

## Ramas de actualización automatizadas

Los flujos de trabajo crean pull requests utilizando las siguientes convenciones de nombres para las ramas:

- Actualizaciones de paquetes AUR: `aurbump-<name>`
- Actualizaciones de otros paquetes: `othersbump-<name>`
- Actualizaciones de imágenes Docker en este repositorio: `dockerbump-<name>`
- Actualizaciones de imágenes Docker en repositorios externos: ramas existentes por imagen, como `alpine`, `golang` y `archlinux`

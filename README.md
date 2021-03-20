# Assets

Ficheros con datos y recursos comunes para los clientes de gatovid y su
comunicación con el backend.

Este repositorio debería añadirse como un submódulo en git para que se mantenga
la misma estructura en todos los clientes.

Se añade a continuación un tutorial rápido sobre cómo usar los submódulos de
Git, que son simplemente repositorios dentro de repositorios:

## Añadir submódulo

Para añadir el submódulo al proyecto git:

```sh
$ git submodule add git@github.com:UNIZAR-30226-2021-07/assets.git [DIRECCION]
```

Se puede usar una dirección destino si se especifica un `DIRECCION`. Por
ejemplo, para que este directorio se guarde como `app/assets/common`, se le
daría ese valor respecto a la ruta actual en la que te encuentras.

## Actualizar repositorio

Para actualizarlo después de que se hayan añadido cambios a este repositorio,
puedes hacer:

```sh
$ git submodule update
```

O directamente entrar en la carpeta en la que se sitúe este repositorio y hacer:

```sh
$ git pull
```

## Descargar tras `git clone`

Posteriormente, cuando clones el repositorio principal la carpeta con este
repositorio estará vacía o será inexistente. Para clonar los submódulos por
primera vez se puede usar, dentro del proyecto Git que los tenga:

```sh
$ git submodule init
$ git submodule update
```

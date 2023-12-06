# Proyecto de ejemplo de uso de Nexus OSS con Docker Compose

Disponemos de un compose.yaml que nos permite gestioanr un servicio nexus

## Requisitos
Necesitamos tener instalado Docker y Docker Compose

## Descargamos el repositorio y nos movemos al directorio

## Arranque de nexus

```shell
docker compose up -d
```

## Acceso 
Podemos acceder con el usuartio admin a [http://localhost:8081/](http://localhost:8081/)
La contraseña la podemos encontrar en el fichero admin.password de la carpeta nexus-data

## Despliegue del artefacto SNAPSHOT
Ejecutamos el despliegue
```shell
 mvn clean deploy -Dmaven.test.skip=true
```

## Verificamos el contenido desde Nexus desde el repositorio Snapshots

## Cambiamos a una versión 1.0-FINAL

## Despliegue del artefacto RELEASE
Ejecutamos el despliegue
```shell
 mvn clean deploy -Dmaven.test.skip=true
```

## Verificamos el contenido desde Nexus en el repositorio Releases


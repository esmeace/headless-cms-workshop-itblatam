# Instalación de ContentBox

Si instaló correctamente Docker, copie nuestro archivo `docker-compose.yml` en `HeadlessContentBox`. 
Luego CD en el directorio `HeadlessContentBox`.

```
cd HeadlessContentBox
```
## Asistente de instalación de ContentBox
Comencemos la instalación de ContenBox usando el asistente de instalación.

```
contentbox install-wizard
```
Se le solicitará lo siguiente:

1. ¿Cuál es el nombre del sitio que desea crear?  cbheadless
2. ¿En qué motor CFML se ejecutará el sitio? Seleccione Lucee 5
3. Ingrese la contraseña para el administrador de CFML Engine (déjelo en blanco para usar 'contentbox', solo si se implementa en CommandBox)? (Déjelo en blanco)
4. Ingrese la contraseña para ColdBox HMVC Reinits (déjelo en blanco para usar 'contentbox')? ( Déjelo en blanco )
5. ¿Qué base de datos utilizará? Seleccione MySQL 8 + (Asegurece que la X este en el cuadro de selección)
6. Ingrese el host de la base de datos (déjelo en blanco para usar 'localhost')? mysql ( si usa Docker )
7. Ingrese el puerto de la base de datos (déjelo en blanco para usar el predeterminado para MySQL8)? ( Déjelo en blanco )
8. Ingrese el nombre de usuario de la base de datos para usar para la conexión. root
9. Ingrese la contraseña de la base de datos para usar para la conexión? itbLATAM2022! ( si usa Docker )
10. Ingrese el nombre de la base de datos a usar para la conexión (déjelo en blanco para usar 'contentbox')? cbheadless
11. ¿Quiere que implementemos e iniciemos un motor CFML (lucee@5) en CommandBox para usted? Seleccione False ( si usa Docker )
12. ¿Es este un sitio de desarrollo o producción? Seleccione Development
13. Ingrese la versión de ContentBox para usar o déjela en blanco para usar la última versión estable (be = snapshot)? ( Déjelo vacio )
14. ¿Desea continuar? [y/n] y

## CORS
Agregar el módulo de CORS para detectar peticiones CORS, esto ayudara a validar las configuraciones del origen y maneja las solicitudes de verificación previa.

```
install cors
```

Salir de CommandBox

```
exit
```

## docker-compose
Construyamos nuestros contenedores MySQL y App.
Asegurarse que Docker este corriendo.
```
docker-compose up -d --build
```

## Base de Datos 
Usando su cliente para manejar su DB MySQL, inicie una nueva conexión.

1. host: 127.0.0.1
2. port: 3357
3. username: root
4. password: itbLATAM2022!

Una vez establecida la conexión, cree una nueva base de datos.
1. name: cbheadless
2. character set: utf8mb4

## Interfaz de usuario del instalador de ContentBox
En su navegador vaya a `http://127.0.0.1:61680/`.  Debería ver el instalador de ContentBox.

## Una vez instalado, puede pasar al siguiente paso
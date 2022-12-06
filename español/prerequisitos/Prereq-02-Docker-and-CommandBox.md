# Configuración de Docker

Docker agrega sus aplicaciones en contenedores para mantenerlas separadas de su infraestructura. 
Descargue e instale el escritorio de Docker, para ejecutar MySQL 8 y nuestra aplicación ContentBox.

https://docs.docker.com/get-docker/

# Configuración de CommandBox

CommandBox es el Cli para CFML que nos ayudará a manejar paquetes/modulos, para este taller lo más importante será usarlo para
installar nuestra aplicación de ContentBox, algunas herramientas de CommandBox y un motor de CFML para ejecutar nuestra aplicación.

## Instalación de CommandBox

Instalar CommandBox no es difícil, pero depende de la configuración de su PC. 
A continuación hay enlaces a la documentación oficial para ayudarlo a través de este proceso.

### Descargar CommandBox

https://commandbox.ortusbooks.com/setup/download

### Instalación de CommandBox

https://commandbox.ortusbooks.com/setup/installation

### Errores comunes de instalación

https://commandbox.ortusbooks.com/setup/common-errors

### Ayuda adicional

El foro de la comunidad es el mejor lugar para comenzar: https://community.ortussolutions.com/

Aunque la comunidad es muy útil, si todo lo anterior no resuelve tus dudas, los canales de Slack para CFML siempre serán muy buena opción, por ejemplo CommandBox King Brad, Box Team y Ortus Community Forum podrían darte la mejor respuesta.

Para este taller también puedes ponerte en contacto con nosotros a través del canal Slack.

## Creación de nuestra aplicación API REST en ColdBox

### Iniciar CommandBox

Inicie CommandBox y luego acceda al directorio

```
box
cd \your\workshop\directory
```

### Instalar [commandbox-bullet-train](https://forgebox.io/view/commandbox-bullet-train)

Una vez inicializado CommandBox deberá installar este modulo:

```sh
install commandbox-bullet-train
```

## Instalar [contentbox-cli](https://www.forgebox.io/view/contentbox-cli)
```sh
instalar contentbox-cli
```

### Reiniciar CommandBox

Al installar módulos, deberá volver a cargar el CLI para cargar los nuevos módulos. 
Ejecutar `r` es un alias para `reload` que reiniciará el cli, esto puede tardar uno o dos minutos.


## Una vez instalado, puede pasar al siguiente paso
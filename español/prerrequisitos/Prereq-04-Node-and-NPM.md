# Instalación de Node y NVM

Instalar Node no es difícil, pero tener la versión correcta de Node en su máquina puede serlo, si tiene aplicaciones que necesitan versiones diferentes a la que necesitaremos en el taller, recomendamos encarecidamente Node Version Manager (NVM) para facilitarle la vida.

## Node Version Manager (Opcional)

Si desea instalar NVM, siga el enlace aquí: https://npm.github.io/installation-setup-docs/installing/using-a-node-version-manager.html

Cuando se instala nvm, puede ejecutar `nvm list` para ver las versiones disponibles para usar.

```
  * 18.12.1 (Currently using 64-bit executable)
    16.13.0
```

Puede instalar versiones adicionales con: `nvm install <version> [arch]`

La versión puede ser una versión específica, "latest" para la última versión actual o "lts" para la versión LTS más reciente. Opcionalmente, especifique si desea instalar la versión de 32 o 64 bits (el valor predeterminado es la arquitectura del SO). Establezca [arch] en "all" para instalar versiones de 32 y 64 bits.  
Agregar `--insecure` al final de este comando para omitir la validación SSL del servidor de descarga remota.

Ejecutar `nvm ?` puede mostrar documentación como la del párrafo anterior.

## Instalación de Node 

Las descargas están disponibles aquí: https://nodejs.org/en/download/

Una vez instalado, debería poder ejecutar el siguiente comando para confirmar la versión

```
node -v
```

Los resultados mostrarán la versión de `v18.12.1`

Ejecutar `npm -v` mostrará la versión de `8.19.2`

## Una vez instalado, puede pasar al siguiente paso
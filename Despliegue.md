# Despliegue PokeDex Angular en Azure App Service

## 1. Creación de la Aplicación Web

Se creó una nueva aplicación web en Microsoft Azure App Service utilizando la suscripción Azure for Students.

Durante la creación se configuraron los siguientes datos:

* Grupo de recursos: rg-listrace-pro
* Nombre de la aplicación: app-listrace-web-prod-despliegue-moron
* Sistema Operativo: Windows
* Tipo de publicación: Code
* Región: East US

Posteriormente se seleccionó la opción **Revisar y crear** y luego **Crear** para iniciar el despliegue del recurso.

---

## 2. Acceso al Recurso Creado

Una vez finalizada la implementación, se ingresó al panel principal del App Service para visualizar la información general del recurso, como estado, dominio predeterminado y configuración inicial.

---

## 3. Preparación del Proyecto Angular

Desde el equipo local se descargó el proyecto `pokedex-angular` y se preparó para producción.

Dentro de la carpeta del proyecto se ejecutaron los siguientes comandos:

npm install

npm run build

El proceso generó la carpeta:

dist/pokedex-angular

La cual contiene los archivos finales listos para publicar.

---

## 4. Publicación en Azure

Luego se ingresó a las herramientas de administración del App Service para cargar los archivos compilados del proyecto.

Se copiaron todos los archivos contenidos en:

dist/pokedex-angular

Y fueron colocados en la carpeta pública del servidor para reemplazar el contenido anterior.

---

## 5. Configuración de Seguridad

Como parte de las buenas prácticas, se verificó la seguridad del sitio mediante la herramienta SecurityHeaders.

Se revisaron encabezados HTTP importantes como:

* Content-Security-Policy
* Strict-Transport-Security
* X-Content-Type-Options
* X-Frame-Options
* Referrer-Policy

Esto permitió validar una configuración más segura para la aplicación web.

---

## 6. Verificación del Despliegue

Finalizado el proceso, se abrió la URL pública del proyecto para comprobar que la Pokédex cargaba correctamente y que la aplicación estaba disponible desde internet sin errores.

---

## URL Final

https://app-listrace-web-prod-despliegue-moron-e0bafra9htgqd2c7.eastus-01.azurewebsites.net

---

## Resultado Final

La aplicación PokeDex fue desplegada exitosamente en Microsoft Azure App Service, quedando accesible públicamente mediante HTTPS y cumpliendo los objetivos del laboratorio.

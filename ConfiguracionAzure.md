# Configuración en Azure

## Introducción

En este documento se presenta la configuración principal utilizada para publicar la aplicación PokeDex en Microsoft Azure App Service.

El objetivo fue dejar la aplicación disponible en internet mediante una URL pública, utilizando recursos en la nube administrados desde Azure Portal.

---

## Servicio Utilizado

Para el despliegue se utilizó el servicio:

**Microsoft Azure App Service**

Este servicio permite alojar aplicaciones web sin necesidad de administrar servidores físicos, facilitando la publicación, monitoreo y acceso desde cualquier lugar.

---

## Información General del Recurso

Durante la creación del servicio se configuraron los siguientes parámetros:

* Tipo de publicación: Code
* Sistema Operativo: Windows
* Estado actual: Running
* Región: East US
* Suscripción: Azure for Students

---

## Datos del Recurso Creado

* Nombre de la aplicación: app-listrace-web-prod-despliegue-moron
* Grupo de recursos: rg-listrace-pro
* Plan de hospedaje: ASP-rglistraceprod-aac9

Estos recursos fueron creados desde el portal de Azure para alojar la aplicación correctamente.

---

## Dominio Público

Una vez completada la configuración, Azure generó automáticamente el siguiente dominio público:

https://app-listrace-web-prod-despliegue-moron-e0bafra9htgqd2c7.eastus-01.azurewebsites.net

Desde esta dirección se puede acceder a la aplicación en cualquier momento.

---

## Validación del Servicio

Después del despliegue se verificó:

* Acceso correcto desde navegador web.
* Funcionamiento general de la aplicación.
* Disponibilidad mediante HTTPS.
* Estado activo del recurso en Azure.

---

## Resultado Final

La configuración en la nube fue completada exitosamente, permitiendo publicar la aplicación PokeDex en Microsoft Azure y dejándola disponible para acceso público.

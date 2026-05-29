# Infraestructura-Nube
# Práctica: Control de la Nube con gcloud CLI

Alumno: Jose Eduardo Santos Toribio
Materia: Infraestructura en la Nube
Tema: Configuración de gcloud CLI en Ubuntu
Fecha: 28 de mayo de 2026

## Introducción

La herramienta gcloud CLI permite administrar servicios de Google Cloud Platform desde la terminal de comandos. Su uso es fundamental en entornos profesionales debido a que facilita la automatización, configuración y administración de infraestructura en la nube sin depender de interfaces gráficas.

Actualmente, la mayoría de las organizaciones utilizan plataformas de nube pública para desplegar aplicaciones, almacenar información y administrar servicios digitales. Por esta razón, aprender a utilizar herramientas de línea de comandos como gcloud CLI es una habilidad esencial para cualquier profesional relacionado con infraestructura, virtualización y computación en la nube.

## Objetivo

Instalar, inicializar y verificar la configuración de gcloud CLI en Ubuntu, estableciendo correctamente la autenticación, el proyecto y la zona de trabajo.

## Desarrollo de la práctica

### Instalación de Google Cloud CLI

Primero se actualizó el sistema operativo Ubuntu y posteriormente se instaló el paquete oficial de Google Cloud CLI mediante el gestor de paquetes apt-get.

Comando utilizado:

```bash
sudo apt-get update && sudo apt-get install google-cloud-cli
```

### Inicialización y autenticación

Después de completar la instalación, se ejecutó el comando de configuración inicial para vincular la terminal con una cuenta institucional de Google Cloud Platform.

Comando utilizado:

```bash
gcloud init
```

Durante este proceso se abrió un enlace de autenticación en el navegador donde se inició sesión con la cuenta correspondiente. Posteriormente se seleccionó el proyecto asignado y se configuró la zona geográfica predeterminada.

### Configuración de zona

Se estableció como zona principal:

```bash
us-central1-a
```

La selección de una zona es importante debido a que los recursos de nube se ejecutan físicamente en centros de datos específicos distribuidos alrededor del mundo.

### Verificación de la configuración

Finalmente, se verificó el estado de la configuración activa mediante el siguiente comando:

```bash
gcloud config list
```

Este comando permitió comprobar correctamente:

* La cuenta autenticada
* El proyecto configurado
* La zona geográfica seleccionada

## Resultado obtenido

La práctica se realizó correctamente, logrando autenticar la cuenta en Google Cloud y configurar adecuadamente el entorno de trabajo. La herramienta gcloud CLI quedó lista para futuras actividades relacionadas con despliegue y administración de infraestructura en la nube.


```bash
gcloud config list
```

## Conclusión

El uso de gcloud CLI permite gestionar recursos en la nube de forma profesional y eficiente mediante comandos desde la terminal. Esta práctica ayudó a comprender la importancia de la autenticación segura, la organización de proyectos y la configuración geográfica dentro de Google Cloud Platform.

Además, se entendió cómo las herramientas de línea de comandos son esenciales en ambientes reales de trabajo debido a que permiten automatizar procesos y administrar infraestructura de manera rápida y escalable.

## Referencias

Google Cloud. (2026). Google Cloud CLI Documentation. Recuperado de: https://cloud.google.com/sdk/docs

Google Cloud. (2026). Install the gcloud CLI. Recuperado de: https://cloud.google.com/sdk/docs/install

Google Cloud. (2026). gcloud CLI Overview. Recuperado de: https://cloud.google.com/sdk/gcloud

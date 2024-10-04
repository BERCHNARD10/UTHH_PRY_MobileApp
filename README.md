# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).


# Proyecto UTHH_PRY - App Móvil

## Descripción del Proyecto

El proyecto **UTHH_PRY** es una **plataforma de educación móvil** diseñada para facilitar la gestión de aulas virtuales, permitiendo a los estudiantes realizar actividades como la creación de **materias**, **gestión de actividades y prácticas**, y el acceso a **notificaciones push en tiempo real**. Además, incluye la funcionalidad de **gestión de calificaciones**, **inicio de sesión**, **perfil** y **recuperación/reestablecimiento de contraseña**.

### Funcionalidades Clave
- **Perfil**: Los usuarios pueden crear y gestionar su perfil personal dentro de la aplicación.
- **Inicio de Sesión**: Los usuarios pueden acceder a la plataforma mediante un sistema seguro de autenticación.
- **Recuperación y Reestablecimiento de Contraseña**: En caso de olvidar la contraseña, los usuarios pueden recuperarla o reestablecerla.
- **Materias**: Los docentes pueden crear materias y organizarlas para gestionar el contenido y las evaluaciones.
- **Actividades y Prácticas**: Los docentes pueden asignar tareas y prácticas, y los estudiantes pueden completarlas directamente desde la app.
- **Detalle de Práctica**: Los estudiantes pueden acceder a los detalles de cada práctica asignada.
- **Notificaciones Push en Tiempo Real**: Los estudiantes reciben notificaciones sobre nuevas asignaciones, calificaciones, y otras actualizaciones importantes, incluso cuando la aplicación está cerrada.

## Objetivo General

Este proyecto consiste en el desarrollo de una aplicación móvil basada en **React Native** que incluye un sistema de **notificaciones push en tiempo real**, junto con módulos como el perfil de usuario, inicio de sesión, actividades, y gestión de calificaciones. El objetivo es ofrecer una experiencia similar a una app nativa que permita a los usuarios acceder a las funciones clave de la plataforma educativa de manera fluida y eficiente.


## Estructura del Proyecto

El proyecto sigue una arquitectura basada en tres capas:
1. **Frontend**: Implementado en **React Native** utilizando componentes nativos y Javascript para ofrecer una experiencia fluida en dispositivos móviles.
2. **Backend**: Implementado en PHP con una API tipo REST para gestionar datos y autenticar usuarios.
3. **Base de Datos**: **MySQL** es utilizada para gestionar la información de usuarios, actividades, materias, y calificaciones.

## Metodología de Trabajo

Este proyecto utiliza **Extreme Programming (XP)** para fomentar la comunicación y colaboración constante dentro del equipo. Además, implementa **Trunk-Based Development** como estrategia de versionamiento, permitiendo integrar pequeñas actualizaciones frecuentes en la rama principal.

- **Revisiones frecuentes de código** mediante **pair programming**.
- **Pruebas continuas** para asegurar la calidad de cada nuevo cambio antes de integrarlo.
- **Feedback del cliente** para ajustar los objetivos del proyecto a las necesidades cambiantes.

### Ciclos de Iteración:
Cada iteración tiene una duración de 1-2 semanas, y al final de cada iteración se realiza una reunión de retrospectiva para evaluar el progreso y ajustar las prioridades. Los entregables se revisan constantemente con el cliente.

## Control de Versiones

El proyecto utiliza **Git** como sistema de control de versiones y sigue el flujo de trabajo de **Trunk-Based Development**.

### Estrategia de Versionamiento:
- El desarrollo de cada funcionalidad se realiza en ramas **temporales** cortas que se derivan de la rama principal (`main`).
- Las ramas siguen la convención `feature/nombre-de-la-funcionalidad`. Ejemplos:
- `feature/animaciones-funcionalidades`
- `feature/apis-logica-negocio`
- `feature/componentes-UI`
- `feature/limpieza-y-optimizacion-codigo`
- `feature/mejoras-rendimiento`
- `feature/navegacion-pantallas`
- `feature/pantallas-principales`
- `feature/pruebas-y-optimizacion`
- `master`

- **Integración frecuente**: Las ramas deben fusionarse rápidamente a `master` una vez que el código haya sido revisado y probado.
- **Revisión de código**: Se realiza una revisión de código por al menos un miembro del equipo antes de fusionar la rama.


### Flujo de Trabajo:
1. **Crear una nueva rama** para cada funcionalidad o tarea específica.
```bash
git checkout -b feature/nombre-de-la-funcionalidad
```
2. **Hacer commits** frecuentes de los cambios.
```bash
git add .
git commit -m "Descripción del cambio"
```
3. **Abrir un pull request** para revisión de código por otro miembro del equipo.
```bash
git checkout main
```
4. **Integrar la rama** en `main` después de que las pruebas automáticas pasen y el código sea aprobado.
```bash
git merge feature/nombre-de-la-funcionalidad
```

## Estrategia de Despliegue
Para el despliegue del proyecto, se ha seleccionado la estrategia de **Rolling Deployment**, que permite realizar actualizaciones de la aplicación sin tiempos de inactividad.

### Entornos de Despliegue Definidos:
1. **Desarrollo**: Aquí se realizan las primeras pruebas de las funcionalidades iniciales y desarrollo activo.
2. **Staging**: Réplica del entorno de producción donde se realizan las pruebas finales antes del despliegue.
3. **Producción**: El entorno en el que la aplicación está disponible para los usuarios finales.

## Proceso de CI/CD
Se utiliza **Integración Continua (CI)** para asegurar que cada cambio que se integra al tronco principal pase por un proceso automatizado de pruebas. Cuando todas las pruebas pasan, el código se despliega automáticamente en los entornos de **Staging** y posteriormente en **Producción**.

## Instrucciones para Contribuir

1. **Clonar el repositorio**: Esto descargará una copia del código fuente en tu máquina local.
```bash
git clone https://github.com/BERCHNARD10/UTHH_PRY_MobileApp
```
2. **Entrar en el directorio del proyecto**: Accede al directorio clonado donde está el código del proyecto.
```bash
cd UTHH_PRY_MobileApp
```
3. **Instalar dependencias**: Esto instalará todas las dependencias necesarias del proyecto especificadas en package.json.
```bash
npm install
```
4. **Ejecutar el proyecto en modo desarrollo**: Inicia el servidor en modo desarrollo. Esto te permitirá ver la aplicación en tiempo real y se recargará automáticamente cuando realices cambios en el código.
```bash
npx expo start
```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.

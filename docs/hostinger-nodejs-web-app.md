# Cómo agregar una aplicación web Node.js en Hostinger

Guía paso a paso para desplegar aplicaciones Node.js en Hostinger mediante integración con GitHub o carga de archivos.

## Planes compatibles con aplicaciones Node.js

Las aplicaciones web Node.js están disponibles en los siguientes planes:

- Business Web Hosting
- Cloud Startup
- Cloud Professional
- Cloud Enterprise
- Cloud Enterprise Plus

> Nota: Los planes VPS y servidores dedicados también soportan Node.js, pero requieren configuración manual por línea de comandos.

## Requisitos

- Un plan Business o Cloud (Cloud Startup, Cloud Professional, Cloud Enterprise o Cloud Enterprise Plus).
- Una app Node.js basada en un framework compatible.
- Repositorio en GitHub o archivos del proyecto comprimidos.

## Frameworks y tecnologías compatibles

**Aplicaciones frontend:**

- React
- Vue.js
- Angular
- Vite
- Parcel
- Preact
- Next.js

**Aplicaciones backend:**

- Next.js
- Express.js

**Versiones de Node.js compatibles:** 18.x, 20.x, 22.x, 24.x.

## Despliegue desde un repositorio de GitHub

1. **Accede a la sección de Node.js Web App**
   - Inicia sesión en hPanel.
   - Ve a **Websites** y selecciona **Add Website**.

2. **Selecciona Node.js Web App**
   - Elige **Node.js Apps** en las opciones disponibles.

3. **Elige integración con GitHub**
   - Selecciona **Import Git Repository**.

4. **Autoriza el acceso a GitHub**
   - Serás redirigido a GitHub.
   - Haz clic en **Authorize** para permitir el acceso a tus repositorios.

5. **Selecciona tu repositorio**
   - Escoge el repositorio que contiene tu aplicación Node.js.

6. **Configura los ajustes de build**
   - El sistema detectará el framework y sugerirá los ajustes.
   - Ajusta los valores si es necesario.

7. **Despliega tu sitio**
   - Haz clic en **Deploy** para iniciar el build.
   - Se publicará en un subdominio temporal por defecto.

✅ ¡Tu app Node.js estará en línea!

## Despliegue subiendo archivos

1. **Accede a la sección de Node.js Apps**
   - Inicia sesión en hPanel.
   - Ve a **Websites** y selecciona **Add Website**.

2. **Selecciona la aplicación frontend**
   - Elige **Node.js Apps**.

3. **Elige carga de archivos**
   - Selecciona **Upload your website files**.

4. **Sube tu proyecto**
   - Carga un archivo comprimido (.zip) que contenga tu app Node.js.

5. **Configura los ajustes de build**
   - Confirma o edita los ajustes detectados automáticamente.

6. **Despliega tu sitio**
   - Haz clic en **Deploy** para compilar y publicar.

✅ ¡Tu sitio ya está listo!

## Administración de tu app Node.js

### Despliegues desde GitHub

- Verás **Deployment Details** en el dashboard.
- Al entrar, podrás revisar detalles del despliegue.
- Si falla un build, los logs mostrarán el motivo.

### Despliegues por carga de archivos

- Puedes subir nuevos archivos y redeplegar desde el dashboard.
- En **See details** encontrarás la información del despliegue.

## Preguntas frecuentes

### 1. Ya tengo un dominio en Hostinger, ¿cómo despliego Node.js ahí?

Actualmente debes desplegar tu sitio primero como un nuevo website con dominio temporal:

1. **Add Website** y selecciona **Frontend web app**.
2. Elige el método de despliegue (GitHub o carga de archivos).
3. Tras el despliegue, conecta tu dominio o subdominio al temporal con la guía
   **How to Connect a Preferred Domain Name Instead of a Temporary One at Hostinger**.

> Nota: Si el dominio ya está agregado a tu plan de hosting, elimina el website antes de conectarlo.

### 2. ¿Cómo elimino o despublico mi sitio Node.js?

No existe botón de “Stop” o “Delete” para despliegues Node.js. Para dejar el sitio fuera de línea,
se recomienda eliminar el website completo desde hPanel. Esto borrará los despliegues y el sitio.

> Nota: Antes de eliminar, descarga backups. Esta acción no es reversible y se perderán
> archivos, bases de datos, emails y configuraciones.

### 3. ¿Qué comandos npm puedo ejecutar?

No es necesario ejecutar npm manualmente ni instalar NPM por separado. Está preinstalado y los
comandos de build disponibles se muestran en el menú **Build settings** al configurar la app.

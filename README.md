# 🌱 Vivero La Vega - Landing Page

Este repositorio contiene el código fuente de la **Landing Page oficial para Vivero La Vega**. El objetivo de esta web es proporcionar una vitrina digital rápida, moderna y optimizada para buscadores (SEO) que sirva como punto de entrada para los clientes y redirija de forma segura al sistema de gestión interno.

La landing page está construida utilizando el framework **Astro** y desplegada de forma automatizada en la infraestructura global de **Vercel**.

---

## ✨ Características Principales

* **⚡ Rendimiento Superior:** Desarrollada con Astro para lograr tiempos de carga ultra rápidos, excelente retención de usuarios y puntuación óptima en Core Web Vitals.
* **📱 Diseño Totalmente Responsivo:** Adaptada y optimizada al milímetro para su visualización en dispositivos móviles, tablets y computadoras de escritorio.
* **🔍 SEO Optimizado:** Estructura semántica, accesibilidad y metadatos configurados para maximizar la indexación en motores de búsqueda.
* **🛠️ Arquitectura Limpia:** Modularización de componentes Astro y estilos encapsulados para un mantenimiento sencillo.
* **👤 Secciones Dinámicas:** Panel de visualización de roles de usuario (Administrador, Usuario, Empleado) y ventajas competitivas utilizando **Material Icons** de Google.
* **🚀 Despliegue Continuo (CI/CD):** Integración nativa con GitHub y Vercel para actualizaciones automáticas en producción en cuestión de segundos.

---

## 🛠️ Stack Tecnológico

* **Framework:** [Astro](https://astro.build/)
* **Lenguaje:** HTML5, CSS3, JavaScript / TypeScript
* **Iconos:** Material Icons (via Google Fonts)
* **Hosting & Despliegue:** Vercel (Edge Network)
* **Control de Versiones:** GitHub

---

## 🚀 Primeros Pasos

Sigue estos pasos para clonar el proyecto y ejecutarlo en tu entorno de desarrollo local.

### Prerrequisitos

* Tener instalado [Node.js](https://nodejs.org/) (versión 18.x o superior recomendada).
* Un gestor de paquetes de tu preferencia (`npm`, `pnpm` o `yarn`).

### Instalación

1. **Clona el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/vivero-la-vega-landing.git](https://github.com/tu-usuario/vivero-la-vega-landing.git)
   cd vivero-la-vega-landing
   ```
   Instala las dependencias del proyecto:

 ```bash
npm install
# o si usas pnpm: pnpm install
# o si usas yarn: yarn install
```
Configuración de Seguridad y Variables de Entorno
El proyecto utiliza variables de entorno para mapear la redirección hacia el ecosistema del sistema de gestión sin exponer URLs duras en el código fuente.

Crea un archivo llamado .env en la raíz de tu proyecto.

Añade la variable que apunta al subdominio de tu sistema (alojado en tu VPS de Hostinger):

Code snippet
PUBLIC_SYSTEM_URL
⚠️ Nota de Seguridad Crítica: El archivo .env se encuentra estrictamente registrado dentro de .gitignore. Esto evita de forma proactiva que información sensible, credenciales o configuraciones locales sean expuestas públicamente en GitHub.

Desarrollo Local
Para levantar el servidor de desarrollo local con recarga en vivo (Hot Module Replacement), ejecuta:

 ```bash
npm run dev
```
Una vez iniciado, abre tu navegador en la dirección local indicada en la terminal (usualmente http://localhost:4321).

Compilación para Producción
Para generar el build estático y optimizado listo para producción:

 ```bash
npm run build
```
El resultado ultra comprimido se depositará de forma automática en el directorio /dist.

## 📦 Flujo de Despliegue Continuo (CI/CD)
La arquitectura del proyecto está conectada directamente con Vercel para gestionar el ciclo de vida del software de manera profesional:

Producción: Cada git push a la rama principal (main o master) compila el proyecto automáticamente y actualiza la web oficial en viveros-web.devxsota.cloud en menos de un minuto.

Vistas Previas (Previews): Los cambios subidos a ramas de desarrollo secundarias generarán una URL de entorno seguro independiente, ideal para realizar pruebas en dispositivos reales antes de realizar el merge definitivo a producción.

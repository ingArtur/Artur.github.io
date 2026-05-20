# Portafolio Personal — Artur Aroca

Sitio web personal que presenta mi perfil profesional, proyectos y trayectoria como desarrollador. Construido con **HTML, CSS y JavaScript**, con un backend ligero en **Node.js** y desplegado en contenedor **Docker** detrás de **Nginx**.

🌐 **Sitio en vivo:** [https://ingartur.github.io/Artur.github.io/](https://ingartur.github.io/Artur.github.io/)

---

## Tabla de contenidos

- [Descripción](#descripción)
- [Características](#características)
- [Tecnologías](#tecnologías)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Instalación local](#instalación-local)
- [Despliegue con Docker](#despliegue-con-docker)
- [Contacto](#contacto)

---

## Descripción

Este portafolio es mi carta de presentación pública como **estudiante de Ingeniería de Software y Tecnólogo en Análisis y Desarrollo de Software**. Incluye:

- Resumen profesional y formación.
- Stack tecnológico actual.
- Proyectos destacados con enlaces a sus repositorios.
- CV descargable en PDF.
- Información de contacto directo.

El sitio está optimizado para SEO (con `sitemap.xml` y `robots.txt`), preparado para producción con Nginx, y empacado en una imagen Docker para portabilidad.

## Características

- **Diseño responsive** adaptado a móvil, tablet y escritorio.
- **CV integrado** disponible para descarga directa.
- **SEO básico configurado:** sitemap, robots.txt y metadatos.
- **Servidor Node.js** para servir contenido en local.
- **Imagen Docker lista para producción** servida con Nginx.
- **Variables de entorno** configurables mediante archivo `.env`.

## Tecnologías

| Categoría | Tecnología |
|---|---|
| Frontend | HTML5, CSS3, JavaScript |
| Backend | Node.js |
| Servidor web | Nginx |
| Contenedores | Docker |
| Despliegue | GitHub Pages |

## Estructura del proyecto

```
Artur.github.io/
├── css/                  # Hojas de estilo
├── js/                   # Scripts del cliente
├── image/                # Recursos gráficos
├── docker/               # Configuración de contenedores
├── index.html            # Página principal
├── server.js             # Servidor Node.js
├── nginx.conf            # Configuración de Nginx
├── robots.txt            # Directivas para crawlers
├── sitemap.xml           # Mapa del sitio para SEO
└── Curriculum__.pdf      # CV descargable
```

## Instalación local

**1. Clonar el repositorio**

```bash
git clone https://github.com/ingArtur/Artur.github.io.git
cd Artur.github.io
```

**2. Instalar dependencias**

```bash
npm install
```

**3. Configurar variables de entorno**

Copiar la plantilla y completarla con tus valores:

```bash
cp .env.example .env
```

**4. Ejecutar el servidor**

```bash
node server.js
```

El sitio quedará disponible en `http://localhost:3000` (o el puerto configurado en `.env`).

## Despliegue con Docker

El proyecto incluye configuración Docker para despliegue en producción. La guía completa está en [`DOCKER_DEPLOYMENT_GUIDE.md`](DOCKER_DEPLOYMENT_GUIDE.md).

**Construcción rápida:**

```bash
docker build -t artur-portfolio .
docker run -d -p 80:80 artur-portfolio
```

## Contacto

**Artur Andrés Aroca Yara**

- 🌐 Portafolio: [ingartur.github.io/Artur.github.io](https://ingartur.github.io/Artur.github.io/)
- 💼 LinkedIn: [Artur Andrés Aroca Yara](https://www.linkedin.com/in/artur-andres-aroca-yara-565363272)
- 📧 Email: arthurandres30@gmail.com
- 🐙 GitHub: [@ingArtur](https://github.com/ingArtur)

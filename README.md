<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0A66C2,100:00D9FF&height=200&section=header&text=Wilver%20Xi%C3%A1%20Ixcot&fontSize=46&fontColor=ffffff&fontAlignY=42&desc=Desarrollador%20Backend%20Junior&descSize=20&descAlignY=64" alt="Wilver Xiá Ixcot" width="100%" />

**Python · FastAPI · PostgreSQL · React**

Ingeniero en Sistemas · Quetzaltenango, Guatemala 🇬🇹

<br>

[![Portafolio](https://img.shields.io/badge/Portafolio-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white)](https://portafoliowxi.netlify.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/wilveremilio)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ixcotwilver@gmail.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/50259826624)

</div>

<br>

## 👨‍💻 Sobre mí

Construyo **APIs REST con Python y FastAPI**, diseño bases de datos relacionales y desarrollo interfaces con **React y Next.js**. He trabajado en el backend de un sistema de gestión municipal con datos geoespaciales y en proyectos freelance, del backend al frontend.

| | |
|---|---|
| 🎯 **Busco** | Posición junior de backend o full stack |
| 🔨 **Trabajando en** | Base de datos de un sistema de control de inventario |
| 🎓 **Formación** | Ingeniería en Sistemas, Universidad Mesoamericana (pensum cerrado) |
| 🌐 **Idiomas** | Español nativo · Inglés A2 (en mejora) |

<br>

## 🛠️ Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,fastapi,postgres,mysql,nodejs,js,ts,react,nextjs,astro,tailwind,html,css,git,github,docker,linux&perline=9" alt="Stack tecnológico" />

</div>

| | |
|---|---|
| **Backend** | Python, FastAPI, SQLAlchemy, Node.js, APIs REST, JWT |
| **Frontend** | React, Next.js, Astro, TypeScript, Tailwind CSS, Vite |
| **Datos** | PostgreSQL, MySQL, SQL Server, PostGIS, modelado y normalización |
| **Otros** | Git/GitHub, Docker, Postman, Linux, Strapi (CMS), Stripe (pagos) |

<br>

## 🚀 Proyectos

### 📦 Sistema de control de inventario · *en desarrollo*

Base de datos para una empresa que fabrica y distribuye productos de limpieza (caso de negocio simulado): compras, producción por lotes, envasado, ventas en ruta, crédito y cobros.

![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=databricks&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)

- **Trazabilidad completa:** de una venta al lote de producción y, desde ahí, a los lotes de insumo.
- **Existencias calculadas, no editadas:** solo cambian por movimientos de inventario.
- **Auditoría y roles:** transacciones que se anulan con motivo (no se borran) y bitácora de cambios.
- **Estado:** diseño conceptual completo; implementación de tablas en curso, empezando por seguridad y catálogos.

<details>
<summary><b>Ver diagrama conceptual (simplificado)</b></summary>

```mermaid
erDiagram
    PROVEEDOR ||--o{ COMPRA : recibe
    COMPRA ||--|{ DETALLE_COMPRA : contiene
    INSUMO ||--o{ DETALLE_COMPRA : "se compra en"
    DETALLE_COMPRA ||--o{ LOTE_INSUMO : genera
    PRODUCTO ||--o{ LOTE_PRODUCCION : "se fabrica en"
    LOTE_PRODUCCION }o--o{ LOTE_INSUMO : consume
    CLIENTE ||--o{ VENTA : realiza
    VENTA ||--|{ DETALLE_VENTA : contiene
    LOTE_PRODUCCION ||--o{ DETALLE_VENTA : "origen de"
    VENTA ||--o{ ABONO : recibe
```

</details>

<!-- TODO: cuando subas el repo, agrega aquí el enlace: [📂 Ver repositorio](URL) -->

<br>

### 🗺️ Sistema de gestión municipal · *backend*

Backend de un sistema para la Municipalidad de Palestina de Los Altos, con visualización en mapas de la red de agua potable.

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![PostGIS](https://img.shields.io/badge/PostGIS-336791?style=flat-square&logo=postgresql&logoColor=white)

- **17 endpoints REST** usados por 10 usuarios.
- **Datos geoespaciales con PostGIS:** ubicar una tubería pasó de **45 a 10 minutos**.
- Pruebas y documentación técnica para capacitar al equipo.

<br>

### 🛒 E-commerce Marta · *full stack*

Tienda en línea con catálogo, carrito, checkout y pagos con Stripe. Contenido administrado con Strapi.

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Strapi](https://img.shields.io/badge/Strapi-2F2E8B?style=flat-square&logo=strapi&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-008CDD?style=flat-square&logo=stripe&logoColor=white)

<br>

### 🏨 Hotel Horiani · *propuesta freelance*

Propuesta técnica de un sistema de gestión hotelera (FastAPI, PostgreSQL, React) con sitio web público en Astro, actualmente en construcción.

<br>

## 💼 Experiencia

**Desarrollador Backend** · Municipalidad de Palestina de Los Altos · 06/2025 – 12/2025

- Desarrollé APIs REST con Python y FastAPI y modelé la base de datos relacional en PostgreSQL.
- Procesé datos geoespaciales con PostGIS para visualizar la red de agua potable en mapas.
- Realicé pruebas y documenté el sistema para capacitar al equipo.

**Desarrollador Full Stack (freelance)** · E-commerce Marta · 06/2024 – 12/2024

- Construí el frontend con React, TypeScript y Next.js; integré Stripe y Strapi.

<br>

## 📚 Formación

- **Ingeniería en Sistemas**, Universidad Mesoamericana · 2021 – 2025 · pensum cerrado
- **Cursos:** React y Servicios web con Python y FastAPI (Código Facilito) · Bases de datos (TodoCode)

<br>

<!--
OPCIONAL: estadísticas de GitHub. Actívalas solo cuando tu actividad pública sea sólida
y el servicio responda bien. Quita las marcas de comentario para usarlas.

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=WILVEREMILIO&show_icons=true&hide_border=true" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=WILVEREMILIO&layout=compact&hide_border=true" />
</div>
-->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:00D9FF,100:0A66C2&height=90&section=footer" width="100%" alt="" />

</div>

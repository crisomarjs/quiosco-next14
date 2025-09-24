# 🍔 Quiosco de Comida - Next.js 14

Aplicación web de un **quiosco de comida** desarrollada con **Next.js 14 (App Router)** y **Prisma**.  
El sistema permite a los usuarios **realizar pedidos**, al administrador **gestionar productos** y **controlar las órdenes en tiempo real**.  

---

## 🚀 Tecnologías utilizadas

- Next.js 14 con **App Router**
- TypeScript
- Prisma como ORM
- PostgreSQL como base de datos
- TailwindCSS para estilos
- Cloudinary para almacenamiento de imágenes
- SWR para data fetching y revalidación automática
  
---

## 📦 Instalación

Clona el repositorio:

```bash
git clone https://github.com/crisomarjs/quiosco-next14
cd quiosco-next14
npm install
````
---

## ⚙️ Configuración de variables de entorno

Crea un archivo .env en la raíz con la configuración de tu base de datos y otras variables necesarias para la conexión a Cloudinary:
```bash
DATABASE_URL=tu_url_bd
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
NEXT_PUBLIC_CLOUDINARY_API_KEY
CLOUDINARY_API_SECRET=
````

---

## 📂 Estructura del proyecto

```bash
app/                # Rutas principales
 ├── admin/         # Panel de administración
 ├── order/         # Flujo de pedido del cliente
 ├── orders/        # Listado de órdenes activas
 ├── products/      # Gestión y visualización de productos
 ├── layout.tsx     # Layout global
 └── page.tsx       # Página inicial del kiosco

components/         # Componentes reutilizables
 ├── admin/
 ├── order/
 ├── products/
 └── ui/

prisma/             # Esquemas y migraciones de base de datos
public/             # Archivos estáticos (imágenes, íconos)
src/                # Código fuente adicional
 ├── lib/           # Funciones auxiliares
 ├── schema/        # Validaciones (ej. con Zod)
 ├── types/         # Tipos de TypeScript
 └── utils/         # Funciones utilitarias

````

---

## ✨ Funcionalidades principales
👨‍🍳 Cliente

Visualizar menú de productos (categorías, precios, imágenes).

Agregar productos al carrito.

Realizar pedido desde el kiosco.

🛠️ Administrador

Gestión de productos (crear, editar) con subida de imágenes a Cloudinary.

Visualización de órdenes en tiempo real.

Control del estado de cada pedido.

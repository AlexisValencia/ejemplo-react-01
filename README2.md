# Disoft Servicios Informáticos S.L — Proyecto React

Bienvenido/a al proyecto de ejemplo de **DISOFT Servicios Informáticos S.L**.  
Esta aplicación está desarrollada con **React**, **Vite** y **Tailwind CSS**.

---

## 1. Instalación del entorno y dependencias

### 1.1. Instalación de Node.js y pnpm

- Descarga e instala [Node.js](https://nodejs.org/) (recomendado v18 o superior).
- Instala pnpm (gestor de paquetes rápido y eficiente):

  ```bash
  npm install -g pnpm
  ```

### 1.2. Creación del proyecto con Vite

```bash
pnpm create vite@latest <nombre-de-la-aplicacion>
```
Sigue las instrucciones y elige **React** y **JavaScript**.

### 1.3. Acceso a la carpeta y preparación

```bash
cd <nombre-de-la-aplicacion>
pnpm install
```

---

## 2. Instalación de dependencias principales

### 2.1. React Router DOM

```bash
pnpm install react-router-dom
```

### 2.2. Tailwind CSS, PostCSS y Autoprefixer

```bash
pnpm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

### 2.3. Iconos (opcional, usado en el proyecto)

```bash
pnpm install @iconify/react
```

---

## 3. Configuración de Tailwind CSS

### 3.1. Configura el archivo `tailwind.config.js`:

```js
// tailwind.config.js
module.exports = {
  content: [
    "./index.html",
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### 3.2. Añade las directivas de Tailwind en tu CSS principal (`src/index.css`):

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

## 4. Estructura del Proyecto

- **src/components/**  
  Componentes reutilizables (`Contador`, `CardProducto`, `Modal`, etc).

- **src/pages/**  
  Páginas principales (`Home`, `UseEffectPage`, etc).

- **src/routers/**  
  Configuración de rutas.

- **src/index.css**  
  Archivo principal de estilos (Tailwind).

- **tailwind.config.js**  
  Configuración de Tailwind.

---

## 5. Ejecución del proyecto

### 5.1. Modo desarrollo

```bash
pnpm run dev
```
Abre el navegador en la URL que aparece (por defecto: [http://localhost:5173](http://localhost:5173)).

### 5.2. Build para producción

```bash
pnpm run build
```
Los archivos finales estarán en la carpeta `/dist`.

---

## 6. Funcionalidades principales

- **Página de inicio (Home):**  
  Presentación de la empresa, servicios y valores.

- **Listado de productos:**  
  Cards de productos en un grid responsive y accesible.

- **Contador interactivo:**  
  Componente con botones y modal.

- **Ejemplo de uso de useEffect:**  
  Página que muestra el uso de hooks de React.

- **Botón de volver:**  
  Navegación sencilla entre páginas.

---

## 7. Personalización

- Modifica los productos en el array `productos` en `App.jsx`.
- Cambia textos y colores en los componentes para adaptarlos a tu empresa.
- Agrega nuevas páginas o componentes según tus necesidades.

---

## 8. Notas y soporte

- Si tienes problemas con los estilos, revisa la configuración de Tailwind y la importación del CSS.
- Si usas otro gestor de paquetes (npm o yarn), reemplaza los comandos `pnpm` por `npm` o `yarn`.
- Para dudas o problemas, contacta con el equipo de desarrollo de **DISOFT** o abre un issue en el repositorio.

---
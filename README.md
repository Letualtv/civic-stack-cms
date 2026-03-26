
# Civic Stack CMS

> Plataforma de gestión y transparencia para partidos políticos y agrupaciones ciudadanas.

---

## 🎯 Objetivo del Proyecto

Crear una herramienta integral que facilite la afiliación, la gestión de militantes y la comunicación de propuestas, promoviendo la transparencia y la participación ciudadana.

## ✨ Motivación y Tono
- **Profesionalismo e institucionalidad:** Diseño limpio y seguro.
- **Transparencia:** Secciones públicas para la gestión partidaria.
- **Participación:** Botones de acción destacados: "Afiliarse", "Donar", "Participar".

## 🛠️ Tecnologías y Stack
- **Backend:** Laravel 13 (PHP 8.3)
- **Frontend:** Vue 3 + Inertia.js (SPA)
- **Estilos:** Tailwind CSS
- **Build:** Vite

## 🚀 Instalación Rápida

```bash
git clone https://github.com/tu-org/civic-stack-cms.git
cd civic-stack-cms
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --force
npm install
npm run build
```

## 🏗️ Estructura de Carpetas Principal

- `app/Http/Controllers/` — Controladores de la lógica de negocio
- `app/Models/` — Modelos Eloquent (ej: User)
- `database/migrations/` — Migraciones de tablas: users, jobs, cache, etc.
- `database/seeders/` — Seeders de ejemplo
- `resources/views/` — Vistas Blade (ej: welcome.blade.php)
- `resources/js/` — JS principal y bootstrap de la SPA
- `routes/web.php` — Rutas web principales

## 📂 Rutas y Funcionalidades Clave

- `/dashboard` — Panel de usuario afiliado
- `/admin/settings` — Configuración de identidad del partido (colores, logo, nombre)
- `/admin/militantes` — Gestión de base de datos de militantes

## 🧩 Componentes y Placeholders Sugeridos
- **Propuestas programáticas**
- **Calendario electoral**
- **Hoja de ruta**
- **Portal de transparencia**

## 🖌️ Identidad Visual
- El color principal (`primaryColor`) define la identidad del partido. Úsalo en elementos destacados con `:style="{ backgroundColor: primaryColor }"`.

## 🔒 Seguridad
- Acceso a `/admin` solo para usuarios con rol `admin` (`$page.props.auth.user.role === 'admin'`).

## 🧪 Tests
- Pruebas unitarias y de features en `tests/`
- Ejecuta: `php artisan test`

## 📜 Licencia

MIT

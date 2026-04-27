# Contexto Estratégico del Proyecto: Plataforma para Partidos Políticos

## 🎯 Objetivo del Proyecto
- Crear una herramienta integral de gestión y transparencia para **partidos políticos y agrupaciones ciudadanas**.
- La web debe facilitar la afiliación, la gestión de bases de datos de militantes y la comunicación de propuestas.

## ✨ Motivación y Tono
- **Profesionalismo y Confianza:** El diseño debe ser limpio, institucional y transmitir seguridad.
- **Transparencia:** Fomentar secciones donde el ciudadano pueda ver la gestión del partido.
- **Participación:** Priorizar botones de acción (CTA) como "Afiliarse", "Donar" o "Participar".

## 🛠️ Reglas Técnicas Críticas (Laravel + Vue 3)
- **Identidad Visual:** El color principal (`primaryColor`) representa la identidad del partido. USAR SIEMPRE `:style="{ backgroundColor: primaryColor }"` en elementos destacados.
- **Navegación:** Usar `<Link>` de Inertia.js para una experiencia de Single Page Application (SPA).
- **Seguridad:** El acceso al `/admin` es crítico. Siempre verificar `$page.props.auth.user.role === 'admin'`.

## 📂 Estructura de Rutas
- `/dashboard`: Panel de control del afiliado/usuario.
- `/admin/settings`: Configuración de identidad del partido (colores, logo, nombre).
- `/admin/militantes`: Gestión de base de datos de usuarios.

## 📝 Sugerencias de Contenido
- Al sugerir textos de ejemplo (placeholders), usa frases relacionadas con la política: "Propuestas programáticas", "Calendario electoral", "Hoja de ruta", "Portal de transparencia".
- Iconografía sugerida: `users` (militantes), `clipboard-list` (propuestas), `office-building` (sedes), `identification` (carnet de afiliado).
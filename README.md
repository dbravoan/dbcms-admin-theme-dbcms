# dbravoan/dbcms-admin-theme-dbcms 1.0.0

## Qué hace

`dbravoan/dbcms-admin-theme-dbcms` es un tema de backoffice (`dbcms-admin-theme`). Identifier: `dbcms`. Backoffice oscuro de alta tecnología con acentos neón #00FF99, tipografía monoespaciada y estética cyber-terminal.

## Requisitos y dependencias

- `dbravoan/dbcms-core` `^1.0`

## Instalación y activación

Añade el paquete Composer. Selección del tema admin activo:

- Entorno: `CMS_BRAND` → `config('cms.admin_theme')` (véase `packages/core/config/cms.php`).
- Runtime: `AdminThemeService::getActiveTheme()` / `setActiveTheme()`.
- Durante la instalación web/CLI se elige la marca (`brand`) que fija `cms.admin_theme`.

El identifier del directorio del tema debe coincidir con el valor configurado (p. ej. `dbcms`, `termocms`).

## Configuración

Claves por nombre:

- `CMS_BRAND` / `cms.admin_theme`

Manifest `theme.json` con marca (`brand`: `name`, `tagline`, `logo`, `icon`, `edition`, `accent`, `mode`).

## Rutas

No aplica.

## Comandos Artisan

No aplica.

## Permisos

No aplica.

## Privacidad y datos

No aplica. El layout admin debe mostrar avisos del núcleo (módulo inactivo, errores de sesión, etc.) según el contrato de extensiones.

## Plantillas y assets

- `admin/auth/login.blade.php`
- `admin/dashboard.blade.php`
- `admin/layout.blade.php`
- `assets/admin-bar.css`
- `composer.json`
- `errors/layout.blade.php`
- `theme.css`
- `theme.json`

## Enlaces

- [Extensiones](../../../docs/EXTENSIONS.md)
- [Núcleo y extensiones](../../../specs/CORE_AND_EXTENSIONS.md)
- [README del núcleo](../../../packages/core/README.md)
- [README del monorepo](../../../README.md)

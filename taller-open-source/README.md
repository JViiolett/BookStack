# Taller 02.01 - Análisis de BookStack

Juana Violeta Rojas Espejo
Aplicaciones Open Source - Ingeniería de Software, cuarto semestre
Institución Universitaria de Colombia

Este es un fork de BookStack (https://github.com/BookStackApp/BookStack), la aplicación que analicé para el taller.

En esta carpeta está:

- El informe del taller en Word y en PDF.
- La carpeta `evidencias` con las capturas del repositorio, las carpetas del proyecto y la aplicación funcionando.

## Cómo lo ejecuté

Se necesita PHP 8.3, Composer, MySQL o MariaDB y Node.js.

```
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
npm install
npm run production
php artisan serve --port=8080
```

Antes de hacer `migrate` hay que poner en el archivo `.env` los datos de la base de datos.
Después se entra a http://localhost:8080 con el usuario admin@admin.com y la contraseña password.

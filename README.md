# Comunicacion-BRO

Base nueva de Astro + Vue + Tailwind, copiada del estado local de `navigate-business-web` el 2026-10-22 (HEAD de origen: `8fbc64cb712970c4d04c42931f67f8481159ce37`, con cambios locales). Historial Git independiente, versión inicial `0.1.0`.

## Desarrollo

Requiere Node `^22.13.0 || >=24.0.0` y pnpm.

```sh
pnpm install --frozen-lockfile
pnpm dev
```

```sh
pnpm verify       # ESLint, tipos Astro/Vue y build
pnpm preview     # Vista previa del build
```

## Base conservada

Los cinco archivos `.astro`, `astro.config.mjs`, recursos públicos y ajustes del editor se conservan sin cambios. La página mantiene los textos y la presentación originales de Navigate por petición expresa. La isla Vue muestra `Hello World`, sin autenticación ni llamadas a una API. Los estilos solo eliminan la referencia al directorio `app/` retirado.

Se retiraron `app/`, Firebase, variables de entorno del proyecto anterior, sus aliases, reglas y tests de arquitectura, planes, bitácoras, capturas documentales y la skill local de reconstrucción del acceso. No se copiaron credenciales, dependencias instaladas, builds ni repositorios anteriores.

`docs/fonts/` conserva exactamente las fuentes históricas del original como material de consulta. Describe el proyecto anterior y puede enlazar archivos externos o documentación retirada; no representa funcionalidades de esta base. Las áreas de planes y bitácora quedan limpias para el proyecto nuevo.

La integración Vue y `client:load` se conservan conforme a la [documentación oficial de Astro](https://docs.astro.build/en/guides/framework-components/) (consulta: 2026-10-22). La simplificación de la isla es una adaptación propia a la solicitud actual.

# TalentHub

Aplicación web desarrollada con Angular para gestionar información de empleados Y proyectos.

El proyecto está en desarrollo y se irá ampliando con nuevas funcionalidades.

## Requisitos

- Node.js
- npm

Comprueba que están instalados:

```bash
node --version
npm --version
```

## Instalación

1. Clona o descarga el proyecto.
2. Entra en la carpeta del proyecto.
3. Instala las dependencias:

```bash
npm install
```

## Desarrollo

Inicia el servidor de desarrollo con:

```bash
npm start
```

Después abre `http://localhost:4200/` en el navegador.


## Comandos disponibles

| Comando | Descripción |
| --- | --- |
| `npm start` | Inicia el servidor de desarrollo. |
| `npm run build` | Compila la aplicación. |
| `npm run watch` | Compila y vuelve a compilar al detectar cambios. |
| `npm test` | Ejecuta las pruebas unitarias. |
| `npm run lint` | Comprueba errores de estilo y TypeScript con ESLint. |

## Estructura principal

```text
src/app/
├── core/
│   ├── guards/            
│   ├── interceptors/      
│   └── layout/
│       ├── navbar/
│       └── footer/
├── shared/
│   ├── components/
│   │   ├── spinner/
│   │   ├── avatar/
│   │   └── badge-disponibilidad/
│   └── validators/        
└── features/
    ├── empleados/
    │   ├── models/            
    │   ├── services/
    │   ├── resolvers/
    │   ├── components/
    │   └── index.ts
    ├── proyectos/
    │   ├── models/            
    │   ├── services/
    │   ├── components/
    │   └── index.ts
    └── dashboard/
        ├── components/
        └── index.ts
```

### Organización

- `core/`: artefactos transversales de la aplicacion que normalmente se instancian una unica vez
- `shared/`: elementos reutilizables y genericos que puedes ser usados por distintas partes de la aplicacion
- `features/`: funcionalidades agrupadas por dominio, como empleados o proyectos.
- `models/`: interfaces y tipos de datos.
- `Barrel files`: con index.ts para definir que elementos exponer publicamente de una feature.
- `alias de importacion`: mejoración de la legibilidad de los imports.
- `app.routes.ts`: rutas de la aplicación.
- `styles.scss`: estilos globales.

## Modelos actuales

El proyecto incluye modelos para:

- Empleados.
- Proyectos.

## Estado del proyecto

Proyecto en desarrollo.

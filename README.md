# 🎨 Design System — Dark Mode Color Tokens

Este archivo contiene la definición central de colores para modo oscuro dentro de un sistema de diseño institucional. Su propósito es garantizar consistencia visual, accesibilidad y escalabilidad en interfaces digitales orientadas a entidades públicas y productos con enfoque en experiencia de usuario.

## 📁 Estructura

El archivo `design-color-core.ts` exporta un objeto `dark` con los siguientes grupos de tokens:

- `primary` / `on-primary`: Colores base y contraste para elementos principales.
- `surface` / `on-surface`: Fondos y textos en áreas generales.
- `surface-variant` / `on-surface-variant`: Variantes para componentes secundarios.
- `surface-primary` / `surface-secondary`: Jerarquías visuales en layouts.
- `error` / `on-error`: Indicadores de estado crítico.
- `success` / `on-success`: Confirmaciones y estados positivos.

Todos los valores están definidos en formato hexadecimal, siguiendo criterios de contraste mínimo AA/AAA según WCAG 2.1.

## 🧩 Uso recomendado

Estos tokens pueden integrarse en:

- Sistemas de diseño con soporte para modo claro/oscuro.
- Dashboards institucionales con semáforos de estado.
- Componentes UI reutilizables en frameworks como React, Angular o Vue.
- CSS-in-JS, Tailwind, tokens globales o variables Sass.

Ejemplo de importación:

```ts
import { dark } from './tokens/design-color-core';

const buttonStyles = {
  backgroundColor: dark.primary,
  color: dark['on-primary'],
};

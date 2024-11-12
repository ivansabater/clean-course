# Proyecto para practicar

Este es un proyecto de Vanilla TypeScript en Vite, para trabajar los ejercicios del curso sobre Principios SOLID y CleanCode.

Clonar o descargar el proyecto y luego:

```
yarn install
ó
npm install
```

Para ejecutar el proyecto, simplemente ejecuten

```
yarn dev
ó
npm run dev
```

# Nombre Variables

Tiene que ser pronunciables y expresivos. No usar abreviaturas, a menos que sean muy comunes.
Ejemplo:

```typescript
// Mal
const n = 53;
const tx = 0.15;
const cat = "T-Shirts";
const yyyymmdstr = moment().format("YYYY/MM/DD");

// Bien
const numberOfUnits = 53;
const tax = 0.15;
const category = "T-Shirts";
const birthDate = new Date("1990-01-01");
const currentDate = moment().format("YYYY/MM/DD");
```

## Ausencia de información técnica en nombres

```typescript
// Mal
class AbstractUser {}
class UserMixin {}
class UserImplementation {}
class UserInterface {}

// Bien
class User {}
interface IUser {}
```

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

# Clases

## Comenzar con lista de propiedades

1. Propiedades estáticas
2. Propiedades de instancia
3. Constructor
4. Métodos públicos
5. Métodos privados

## Metodos

1. Empezando por los constructores estáticos
2. Constructores
3. Métodos estaticos.
4. Métodos privados.
5. Métodos de instancia (publicos) ordenados de mayor a menor importancia.
6. Getters y Setters

```typescript
class HtmlElement {
  public static domReady: boolean = false;

  private _id: string;
  private type: stirng;
  private updatedAt: number;

  static createInput(id: string): HtmlElement {
    return new HtmlElement(id, "input");
  }

  constructor(id: string, type: string) {
    this._id = id;
    this.type = type;
    this.updatedAt = Date.now();
  }

  setType(type: string): void {
    this.type = type;
    this.updatedAt = Date.now();
  }

  getId(): string {
    return this._id;
  }
}
```

https://refactoring.guru/

# typescript-tutorial

freeCodeCamp.org

React & TypeScript - Course for Beginners

Source: https://www.youtube.com/watch?v=FJDVKeh7RJI

# examples for using type

example of types, arrays and union operator

```typescript
let name: string;
let age: number | string;
let isStudent: boolean;
let hobbies: string[];
let role: [number, string];

// void return undefined
let printName: (name: string) => void;

// never doesnt return anything
let printName: (name: string) => never;

// not recommended to use "any" type
let something: any;

// unknown is recommanded instead of any
let something: unknown;
```

type declaration and usage for objects

```typescript
type Person = {
  name: string;
  age?: number;
};
let person: Person;
let lotsOfPeople: Person[];
```

example for extension of types

```typescript
type X = {
  a: string;
  b: number;
};

type Y = X & {
  c: string;
  d: number;
};

let y: Y = {
  a: "hello",
  b: 42,
  c: "world",
  d: 404,
};
```

alternative way using interface

```typescript
interface Person {
  name: string;
  age?: number;
}
let person: Person;
let lotsOfPeople: Person[];
```

alternative way using interfaces and extension

```typescript
interface Person {
  name: string;
  age?: number;
}

interface Guy extends Person {
  profession: string;
}

let max: Guy = {
  name: "max",
  age: 28,
  profession: "developer",
};
```

# the typeScript handbook

source: https://www.typescriptlang.org/docs/handbook/intro.html

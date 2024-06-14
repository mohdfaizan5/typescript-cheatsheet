# TypeScript

## Overview

1. Annotations
2. Return Annotation
3. Void in TS

## Never

## Array Types

### Multi Dimensional Arrary

## Objects

## Type alias



## Annotations

Annotations are used to specify a datatype for a variable, parameter, function return value and other types of values
They help developers to catch early errors in development by allowing them to specify what type of values can be assigned to a given variable or passed as an argument to a function.

```ts
// let myVar : datatype = value
```

### String annotations

```ts
let name: string = "faizan";
// we are annotating a variable to use strings

name = "john";

// ❌Error: It will not let you do this
name = 10; // or any other datatype
```

> Note: TypeError : `type "number" is not assignable to type "string"`

### Boolean annotation

```ts
let isAdmin: boolean = false;
```

## Type Inferance

Type inference in TS is a feature that allows the compiler to automatically determine the type of a variable based on its value.
In other words if you declare a variable without explicitly specifing its type. TS will try to infer the type based on the value you assign to it.

```ts
let name = "faizan"; // automatically assign the `string` type to it

name = 20; // this will throw an error
```

## AnyType

TS has a special any type that can be used to represent any type. When a variable is annotated with type `any`, TS will allow it to have any values and will disable all type checking for that variable and its properties.

```ts
let name: any = "Faizan";

name = 20; // It won't complain here as its a type any
name = false;
```

## Function Parameter annotations

They are used to specify the expected types of the parameter that the function takes

```ts
function square(n: number) {
  return n * n;
}

square(5); // ✅
square("faizan"); // ❌ It will not allow for this
```

> Note: Also notice, TS will give you an warning if you provide more or less arguments, that you specify in your parameters area.

- Using Rest parameter

```ts
const myFunction = () => {
  console.log();
};
```

- default parameter

```ts
const myFunction = (name = "Bot") => {
  console.log(name);
};

myFunction("Faizan")
myFunction()
```


## Return Annotation

## Void in TS

## Never

## Array Types

### Multi Dimensional Arrary

## Objects

## Type alias


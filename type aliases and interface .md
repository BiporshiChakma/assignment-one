# Type Alias vs Interface in TypeScript

In TypeScript, both `type` and `interface` are used to define the structure of data. They are quite similar, but they have some differences.

**Interface:** It is mainly used to define the structure of objects. It supports inheritance using `extends` and declaration merging.

**Type Alias:** It is more flexible. It can define objects, strings, numbers, unions, and tuples.

## Example

```typescript
// Interface
interface User {
  name: string;
  age: number;
}

// Type Alias
type Student = {
  name: string;
  age: number;
};

type Status = "active" | "inactive";
```

## Differences of type alias and interface

1. Interface supports declaration merging, but Type Alias does not.
2. Interface uses `extends`, while Type Alias can use `&`.
3. Type Alias supports union types, but Interface does not.
4. Both can define object structures.

## When to Use?

- Use `interface` for defining object structures.
- Use `type` for union types, tuples, and other complex types.

Both are useful in TypeScript. I prefer `interface` for objects and `type` for unions and other types.

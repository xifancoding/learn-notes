# Advanced Type

## `keyof:`

keys of `<T>`. Result is another Type

```typescript
type A = {
    a: string;
    b: number;
    c: boolean;
};
type B = keyof A;       //B = "a" | "b" | "c"
type C = A[B];          //C = string | number | boolean;
```

## `readonly:`

```typescript
type Readonly<T> = {
    readonly [key in keyof T]: T[key];
};
type D = Partial<A>;     //D = { readonly a: string; readonly b: number; readonly c: boolean; }

type DeepReadonly<T> = {
    readonly [key in keyof T]: DeepReadonly<T[key]>;
}
```

## `?:`

? <==> Partial

```typescript
type Partial<T> = {
    [key in keyof T]?: T[key];
};
type D = Partial<A>;     //D = { a?: string; b?: number; c?: boolean; }
```

## `never:`

```typescript
type Pick<T, K extends keyof T> = {
    [key in K]: T[key];
};
type E = Pick<A, "a">;      //E = { a: string };

type Exclude<T, K> = T extends K ? never : T;
type F = Exclude<keyof A, "a">;     //F = "b" | "c";

type Omit<T, K extends keyof T> = Pick<T, Exclude<keyof T, K>>;
type H = Omit1<A, "a">;     //H = { b: number; c: boolean; };
```

...to be continue;

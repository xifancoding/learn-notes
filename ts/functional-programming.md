# functional programming

## `compose:`

...to be continue.

## `curry:`

...to be continue.

## `functor:`

A Functor is a type that implements `map` and obeys some laws. [...more]("https://github.com/MostlyAdequate/mostly-adequate-guide/blob/master/ch08.md#the-mighty-container")

```typescript
//container
type Container<T> = {readonly value: T};

//map type, fn: T -> U;
type MapType = <U>(fn: <T>(value: T) => U) => Container<U>;
```

## `monad:`

...to be continue.

## `applicative:`

...to be continue.

## `.eg`

```typescript
class Just<T> {
    //of functor
    static of = <T>(value: T) => new Just(value);

    //constructor
    public constructor(public readonly value: T) { }

    //map functor, Just<T> -> Just<U>
    public map<U>(fn: (value: T) => U) {
        return Just.of(fn(this.value));
    }
}

//simple promise
// type
```

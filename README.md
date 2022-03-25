# doctest-ts-improved: doctests for TypeScript

Easy doctests for typescript modules, including private methods and extra imports:

```
export default class SomeClass {
    /**
     * Gets the field doubled
     * @example xyz
     *
     * import OtherClass from "./OtherClass";
     * 
     * // Should equal 42
     * SomeClass.get() // => 42
     *
     * SomeClass.get() + 1 // => 43
     * 
     * new OtherClass().doSomething(new SomeClass()) // => 5
     */
    private static get() : number{
        // a comment
        // @ts-ignore
        return 42
    }
}
```

# License

MIT

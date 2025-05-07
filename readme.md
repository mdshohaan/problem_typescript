### Example of using union and intersection types in TypeScript.

    ** 1. Union Type (|) **

> A value that can be one of multiple types.

_✅ Example: Union Type_

````function printId(id: number | string) {
console.log("ID:", id);
}

printId(123); // OK: number
printId("abc123"); // OK: string```

    ** 2. Intersection Type (&)**

> A value that must satisfy multiple types at the same time.
> _✅ Example: Intersection Type_

```type Person = {
name: string;
};

type Employee = {
employeeId: number;
};

type Staff = Person & Employee;

const john: Staff = {
name: "John",
employeeId: 101,
};```
````

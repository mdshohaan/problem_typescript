# 🧑‍💻 Example: Using Union and Intersection Types in TypeScript

This document demonstrates how to use **union** (`|`) and **intersection** (`&`) types in TypeScript.

---

## 1. 🔷 Union Type (`|`)

> A value that can be **one of multiple types**.

✅ **Example: Union Type**

```typescript
function printId(id: number | string) {
  console.log("ID:", id);
}

printId(123); // OK: number
printId("abc123"); // OK: string
```

---

## 2. 🔶 Intersection Type (`&`)

> A value that must satisfy **multiple types at the same time**.

✅ **Example: Intersection Type**

```typescript
type Person = {
  name: string;
};

type Employee = {
  employeeId: number;
};

type Staff = Person & Employee;

const john: Staff = {
  name: "John",
  employeeId: 101,
};
```

---

## ✅ Summary

- **Union Type** allows flexibility by accepting values of multiple types.
- **Intersection Type** ensures that a value must satisfy all combined type conditions.

Use these features to write **type-safe and expressive code** in TypeScript!

# Basic Types

## Syntax

### types

js boolean
`let isDone = false;`
ts boolean
`let isDone: boolean = false;`

generics
`let list: Array<number> = [1,2,3]`

Tuple
let x: [string, number];
x = ["hello", 10];
// red lines for incorrect operations on known indices, operations on unknown indices

enum Color {
    Red,
    Green,
    Blue
}
let c: Color = Color.Green;

// any, any[] Types
// Object types - no methods available

### functions

function in js
function warnUser() {
    console.log("look out!");
}
in ts
function warnUser(): void {}

### falsey values

null and undefined are subtypes of all other types

* under --strictNullChecks, null assigned to any, null type; undefined assigned to any, undefined type, and void

never type

union type: string | null

**declare function...**

### ways around type system

* type assertion

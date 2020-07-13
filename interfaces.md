# Interfaces

interfaces do not allow for undocumented variables

readonly properties (not varibales)
ReadonlyArray<number> -> can override as type assertion...

object literals go through excess property checking
object literal != object instance

**index signature** 
`interface SquareConfig {
    color?: string;
    width?: number;
    // *can have any number of properties of any type*
    [propName: string]: any;
}

**weirdness: object literal assigned to variable not 'excessed' check**

* can pass in object with extra properties as long as have one property in common
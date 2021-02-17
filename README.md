# tiger-full

A compiler for customized tiger language frontend + backend

# Example syntax

```
main let
        type ArrayInt = array [100] of int; /*Declare ArrayInt as a new type */
        var X, Y : ArrayInt := 10; /* Declare vars X and Y as arrays with initialization */
        var i, sum : int := 0;
in
begin
        for i := 0 to 99 do /* for loop for dot product */
                sum := sum + X[i] * Y [i];
        enddo;
        printi(sum); /* library call to printi to print the dot product */
end
```

# Syntax tree

![Syntax Tree](./frontend/tests/loop.png)

## Understanding classes, structs, and records

First of all, it is important to point out that C# is a strongly typed language, so that affects everything we do in code, because we allways need to keep in mind the types of the resources we are using (variables, parameters, references).

In .NET 6 (Visual Studio 2022), you will see warnings when assigning a null value to a property that is not explicitly set as nullable (not declared with `?` sign), although we are able to disable that in the project file (`.csproj`).

Every defined class is a reference type, which means that a variable that points to an instance of this class is pointing to a reference or is a reference to that instance. `class`es can implement `interface`s, which is a contract of properties and methods that the `class` would have. When a `class` implements an `interface`, it also needs to implement all the methods inherited from the `interface`. And a `class` can have its own properties and methods apart from the ones inherited. A `class` can also inherit another `class`, but only one.

We also have `struct`s, which are always `value types`. This means that a variable points to an instance a struct is pointing to the actual object. `struct`s can also implement `interface`s and they can have properties and methods, just like a `class`.

In C# 9, Microsoft introduced the `record` concept, which is behaves very similar to a `class`, but are intended for scenarios where we want to have immutable objects. `record`s can be mutable/changeable but they are useful when we are using them as data objects. A `record` can also do inheritance.

In C# 10 (released with .NET 6), we also have the notion of `record struct`, which aggregates the behaviors and capabilities of both a `record` and a `struct`. 

*Note*: 
- a `record struct` can implement `interface`s but cannot inherit other `struct`s, since they derive from value type.
- when we define a `record`, it is implied that it is a `record class`
## C# compiles to MSIL

C# is one of several .NET languages that compile to Microsoft Intermediate Language (MSIL). Each .NET language has its own compiler that compiles source files (in their particular programming language) to MSIL.

.NET languages:

- F#
- C#
- Visual Basic

Because of this, the C# language can evolve and grow independent of the runtime environment. For example, there are many C# versions (4 - 7.3) that are able to compile to MSIL that can run in .NET Runtime 4. C# versions usually release together with new versions of the compiler.

We can use tools, such as IL Diassembler (ILDASM), to see what the intermediate language is, from a compiled .NET executable or library.

![MSIL/CIL Code](./_images/MSIL-code.jpg)

*MSIL/CIL Code example*
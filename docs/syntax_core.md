# Core syntax
Fractality utilizes Abstract Language (abstractlang) to operate judgments inside and across BBs.

A judgment is written as:

```
C.D:A.B
```

Where **A**, **B**, **C**, **D** are concepts and:
- **`.`** is the relating operator — binds two concepts into a directed relation
- **`:`** is the abstracting operator — the left relation (`C.D`) is declaration, the right (`A.B`) is abstraction

So `engine.car:part.whole` reads: *"'engine to car' is concrete relation of more abstract 'part to whole'"*.

`!engine.gears:part.whole` reads: *"'engine to gears' is NOT a case of 'part to whole'"*.


### Canonical and mirrored forms

A judgment is directed by design but has two equivalent forms:

```
C.D:A.B  ≡  D.C:B.A
```

`engine.car:part.whole` is the same judgment as `car.engine:whole.part`.
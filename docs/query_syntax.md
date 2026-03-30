# Query Syntax

Queries are investigative acts — how a person navigates and interrogates their BB. A query returns concepts, relations, or judgments matching a pattern.

## Expression structure

```
?[polarity]C.D:A.B ::mask
```

## Polarity prefix

| Prefix | Matches |
|---|---|
| `?` or `?+` | positive judgments (default) |
| `?-` | negative judgments |
| `?*` | any polarity |

## Pattern

Follows judgment structure `C.D:A.B`. Use `*` as wildcard for any single concept.

```
?engine.*:*.*       -- judgments where C = "engine", anything else
?*.car:*.*       -- judgments where D = "car"
?*.*:part.whole  -- judgments abstracting over part.whole
```

Concept reference works by title or UUID — no syntax distinction, engine searches both.

## Projection mask

Four bits corresponding to positions **C D A B**. Set `1` to include a position in the result.

| Mask | Returns |
|---|---|
| `::1000` | C |
| `::0100` | D |
| `::0010` | A |
| `::0001` | B |
| `::1100` | C.D (relation) |
| `::0011` | A.B (relation) |
| `::0110` | D,A (comma-separated — not a judgment expression) |
| `::1111` or without mask | C.D:A.B (full judgment, by default) |

Result notation mirrors judgment syntax based on masked positions.

## Logical operators
TBD
Combine patterns within one expression. One mask applies to the whole expression.

| Operator | Meaning |
|---|---|
| `&&` | and |
| `\|\|` | or |
| `!` | not — exclude matching |
| `!!` | xor |



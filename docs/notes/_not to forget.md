Retraction cascades: any relations and concepts left unreferenced after removal are also removed from BB.


One invariant holds across all acts: a BB cannot contain the same judgment in both polarities simultaneously. The acts enforce this naturally.

The Contract is the law of Fractality. Every tool, surface, or pipeline that interacts with BB must comply with it. The Contract does not describe how things are typically done — it prescribes what is valid. Compliance is verifiable; a validator acts as referee between all surfaces.



---

## Scope

The Contract governs all surfaces equally — `.ab` files, CLI, UI, LLM/SLM pipelines. No surface is exempt. The platform (Abstractlang spec and Contract) is versioned independently; each BB pins to a specific version via submodule.


## Piping

```
?<expression>::<mask> | ?<expression>::<mask>
```

Output of the left query feeds into the right query as input. `|` (pipe) is distinct from `||` (logical OR).

## Multi-BB queries

Prefix with a BB address to query across named BBs:

```
@work ?cat.*:*.*::1111                  -- query single BB
@{work,personal} ?cat.*:*.*::1111       -- union query, results tagged by source BB
```

---

## Backlog
- How piped output binds into the next pattern (placeholder syntax TBD)
- `|` vs `||` disambiguation rules TBD

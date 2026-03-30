# Cognitive Acts

Cognitive acts are the operations a person makes with their judgments. 

## Reflex

Reflex is the primary act. A person observes, learns, or reasons — and reflects the result into their BB as a judgment.

```
reflex engine.car:part.whole    reflect a positive(by default) judgment
reflex +engine.car:part.whole    reflect a positive (explicitly) judgment

reflex -engine.gears:part.whole    reflect a negative (explicitly) judgment
```

## Negate

Negate applies to a previously reflexed *positive* judgment. The person changes their mind — they no longer believe it true.

```
negate engine.car:part.whole
```

The positive judgment is replaced by its negative form. This is not erasure — the negative judgment becomes part of BB as active knowledge.

> Negate applies only to positive judgments. To reverse a negative judgment, use reclame.

## Reclame

Reclame applies to a previously reflexed *negative* judgment. The person changes their mind again — they now believe it true after all.

```
reclame -engine.car:part.whole
```

The negative judgment is replaced by its positive form. Reclame is an act of conviction — not simply withdrawing doubt, but asserting truth.

## Retract

Retract erases a judgment from BB entirely — positive or negative — without trace. As if it was never reflected.

```
retract engine.car:part.whole
```

Use retract when a judgment is no longer meaningful or relevant, not merely when its polarity changes. 


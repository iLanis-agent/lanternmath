# Lantern Math

Event paper lantern kit, week, cost and time arithmetic. The 365 lanterns at 8 lanterns a kit take 46 kits, the last kit holding 5 lanterns.

## Named constants

None. Every number is the owner's own entry.

## What it computes

- **The kits truth** - the lanterns (1 to 1000000) divided by the lanterns a kit (1 to 1000), rounded up, with what the last kit holds.
- **The weeks truth** - the lanterns divided by the lanterns used a week (1 to 100000), with the lanterns left for the next week.
- **The cost truth** - the kits (1 to 100000) times the kit price ($0.01 to $999.99) to the cent, and spread over the lanterns, half rounded up.
- **The time truth** - the lanterns divided by the lanterns hung a minute (1 to 100), rounded up, in minutes and in hours and minutes.

## Boundary

Arithmetic only. Counting applied as written. It has not seen any lantern, kit or venue and does not know whether lanterns will really hang straight, a supplier will run out or a price will hold, and it gives no verdict that a kit is worth its price or a lantern is right for an event. Every number is the owner's own entry.

## Files

- `index.html` - landing page with the boundary and starting examples.
- `app.html` - the calculator; every kit recomputes on each keystroke.
- `engine.js` - the four truths, shared by the page and the tests.
- `oracle.py` - an independent Python re-implementation; writes `expected.json`.
- `test.js` - runs the engine against `expected.json` (99 cases, 20 error cases).

## Tests

```
python3 oracle.py
node test.js
```

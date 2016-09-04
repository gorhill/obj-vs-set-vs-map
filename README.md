# obj-vs-set-vs-map
Just a benchmark to measure performance of `Set()`, `Map()` versus `Object.create(null)`.

Run the benchmark for your current browser: <https://gorhill.github.io/obj-vs-set-vs-map/>.

### Example of results

Chromium v51:

- Adding items:
    - `Obj set() x 27.38 ops/sec ±6.75% (50 runs sampled)`
    - `Set set() x 83.31 ops/sec ±3.47% (70 runs sampled)`
    - `Map set() x 68.24 ops/sec ±3.12% (69 runs sampled)`
- Looking up items (80% misses):
    - `Obj get() x 10,516 ops/sec ±0.30% (93 runs sampled)`
    - `Set get() x 17,429 ops/sec ±0.51% (94 runs sampled)`
    - `Map get() x 15,462 ops/sec ±0.35% (96 runs sampled)`
  

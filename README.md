# obj-vs-set-vs-map
Just a benchmark to measure performance of Set(), Map() versus Object.create(null)

Run the benchmark for your current browser: <https://gorhill.github.io/obj-vs-set-vs-map/>.

### Example of results

Chromium v51:

- Adding items:
    - `Obj set() x 26.53 ops/sec ±9.86% (47 runs sampled)`
    - `Set set() x 68.22 ops/sec ±3.69% (70 runs sampled)`
    - `Map set() x 70.71 ops/sec ±3.43% (61 runs sampled)`
- Looking up items (80% misses):
    - `Obj get() x  9,957 ops/sec ±0.41% (96 runs sampled)`
    - `Set get() x 14,789 ops/sec ±0.34% (95 runs sampled)`
    - `Map get() x 14,789 ops/sec ±0.33% (96 runs sampled)`
  

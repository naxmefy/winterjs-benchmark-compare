# winterjs-benchmark-compare

Some benchmarks in comparison to winterjs announced benchmarks.

WinterJS said 150k per sec.

I tried some benchmarks myself.

## Test Command

```bash
wrk -t12 -c400 -d10s http://127.0.0.1:8080
```

## My Mashine

- **Device**: MacBook Pro (13-inch, M1, 2020)
- **Chip**: Apple m1
- **RAM**: 16 GB
- **OS**: Sonoma 14.2.1

## My Results

| Tools              | Req/sec |
| ------------------ | ------- |
| bun                | 212652  |
| deno               | 142687  |
| go (http)          | 196832  |
| ktor               | 16913   |
| node               | 84109   |
| rust (tokio,hyper) | 210826  |

# winterjs-benchmark-compare

Some benchmarks in comparison to winterjs announced benchmarks.

WinterJS said 150k per sec.

I tried some benchmarks myself.

## Test Command

```bash
wrk -t12 -c400 -d10s http://127.0.0.1:8080
```

## Setup 1

- **Device**: MacBook Pro (13-inch, M1, 2020)
- **Chip**: Apple m1
- **RAM**: 16 GB
- **OS**: Sonoma 14.2.1

## Setup 2

- **Device**: MacBook Pro (14-inch, M2, 2023)
- **Chip**: Apple M2 Pro
- **RAM**: 16 GB
- **OS**: Sonoma 14.2.1

## My Results

| Tools              | Req/sec(Setup 1) | Req/sec(Setup 2) |
|--------------------|------------------|------------------|
| bun                | 212652           | 118216           |
| deno               | 142687           | 137932           |
| go (http)          | 196832           | 140812           |
| ktor               | 16913            | 24879            |
| node               | 84109            | 92395            |
| rust (tokio,hyper) | 210826           | 142207           |

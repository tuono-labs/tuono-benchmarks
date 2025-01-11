# Benchmarks

## Results

```
// Tuono
> tuono build

> cargo run --release

> wrk -t12 -c400 -d30s http://localhost:3000/

Running 30s test @ http://localhost:3000/
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    79.72ms  162.90ms   1.71s    87.70%
    Req/Sec    11.50k    15.04k   42.40k    67.36%
  4111435 requests in 30.06s, 3.03GB read
Requests/sec: 136788.14
Transfer/sec:    103.08MB
```

```
// NextJs pages router
> pnpm build

> pm2 start ./ecosystem.config.js

> wrk -t12 -c400 -d30s http://localhost:3000/

Running 30s test @ http://localhost:3000/
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    36.02ms   21.81ms 608.77ms   93.99%
    Req/Sec     0.96k   183.53     3.38k    84.99%
  344202 requests in 30.10s, 493.73MB read
Requests/sec:  11434.43
Transfer/sec:     16.40MB
```

```
// NextJs app router
> pnpm build

> pm2 start ./ecosystem.config.js

> wrk -t12 -c400 -d30s http://localhost:3000/

Running 30s test @ http://localhost:3000/
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    61.03ms   18.65ms 341.31ms   86.25%
    Req/Sec   547.55     96.59     1.16k    80.59%
  195590 requests in 30.10s, 715.91MB read
Requests/sec:   6498.62
Transfer/sec:     23.79MB
```

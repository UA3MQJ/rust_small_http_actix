# rust_small_http_actix

Minimal rust based HTTP server for stress tests

Build:
> cargo build --release

Start:

> target/release/small_http
 
# result 

```
wrk -t100 -c500 -d10s http://127.0.0.1:4000/123

Running 10s test @ http://127.0.0.1:4000/123
  100 threads and 500 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency     4.79ms    3.58ms 133.33ms   97.51%
    Req/Sec     1.05k   269.70     9.81k    92.67%
  1047321 requests in 10.10s, 137.83MB read
  Socket errors: connect 0, read 146, write 0, timeout 0
Requests/sec: 103678.00
Transfer/sec:     13.64MB
```

# Links

https://habr.com/ru/post/324818/

![image](https://github.com/odysee-dev/.github/blob/master/profile/cover.png?raw=true)
# ODY framework

(🚀 Swoole-Powered, Async-First)

ODY is a lightweight high-performance asynchronous PHP framework designed for building microservices and RESTful APIs with ease. Built on top of Swoole, ODY leverages asynchronous processing and coroutines to deliver exceptional performance while maintaining a clean, developer-friendly architecture.

**Warning:**  
🔥 *"After using ODY, going back to Laravel feels like driving a tractor on the Autobahn."*  
*(Yes, it’s that fast. No, it’s not production-ready yet—but you’ll wish it was.)*

Current benchmarks: **33120 requests/sec**
```bash
Running 30s test @ http://localhost:9501/users/1
  12 threads and 200 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency     5.97ms    3.60ms  71.90ms   74.11%
    Req/Sec     2.78k   330.18    12.85k    80.15%
  996776 requests in 30.10s
Requests/sec:  33120.42
```

## Key Features

- **High Performance**: Built with Swoole support for asynchronous processing and coroutines
- **PSR Compliance**: Implements PSR-7, PSR-15, and PSR-17 for HTTP messaging and middleware
- **Modular Design**: Build and integrate different modules
- **Middleware System**: Middleware system for request/response processing
- **Dependency Injection**: Built-in IoC container for dependency management
- **Console Support**: CLI commands for various tasks and application management
- **Routing**: Simple and flexible routing system with support for route groups and middleware

## **🤔 "But Is It Production-Ready?"**
✅ *"We’re almost in beta—but here’s what’s already working:"*
- [x] A solid foundation
- [x] Truly modular design with nex to no dependencies
- [X] WebSockets
- [X] Async CQRS
- [x] AMQP support
- [x] conenction pooling
- [X] 8K RPS benchmarks on lightweight 5$ VPS instances 

**Dare to try it?**
```bash
composer create-project ody/framework ody
cd ody
php ody server:start

curl http://127.0.0.1:9501/users | jq
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   342    0   342    0     0   249k      0 --:--:-- --:--:-- --:--:--  333k
[
  {
    "id": 1,
    "name": "John Doe",
    "email": "john@example.com"
  },
  ...
]
```  

## Documentation

Visit [ody.dev/docs](https://ody.dev/docs) or dive into the packages on this GitHub account,
they contain a lot of information and API references that are not published on the official documentation yet.

## License

ODY Framework is open-source software licensed under the MIT license.


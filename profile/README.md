![image](https://github.com/odysee-dev/.github/blob/master/profile/cover.png?raw=true)
# ODY framework

(🚀 Swoole-Powered, Async-First)

ODY is a lightweight high-performance asynchronous PHP framework designed for building microservices and RESTful APIs with ease. Built on top of Swoole, ODY leverages asynchronous processing and coroutines to deliver exceptional performance while maintaining a clean, developer-friendly architecture.

**Warning:**  
🔥 *"After using ODY, going back to Laravel feels like driving a tractor on the Autobahn."*  
*(Yes, it’s that fast. No, it’s not production-ready yet—but you’ll wish it was.)*

Current benchmarks: **25545.05 requests/sec**
```bash
wrk -t12 -c200 -d30s http://localhost:9501/users/1
Running 30s test @ http://localhost:9501/users/1
  12 threads and 200 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency     8.32ms    6.68ms  72.77ms   82.09%
    Req/Sec     2.14k   169.90     4.01k    69.33%
  767631 requests in 30.05s, 326.44MB read
Requests/sec:  25545.05
Transfer/sec:     10.86MB
```

## 🚀 Key Features

- **High Performance**: Built with Swoole support for asynchronous processing and coroutines
- **PSR Compliance**: Implements PSR-7, PSR-15, and PSR-17 for HTTP messaging and middleware
- **Modular Design**: Build and integrate different modules
- **Middleware System**: Middleware system for request/response processing
- **Dependency Injection**: Built-in IoC container for dependency management
- **Console Support**: CLI commands for various tasks and application management
- **Routing**: Simple and flexible routing system with support for route groups and middleware

## **📦 Batteries Included (But Modular)**
Need more? ODY ships with **13+ modules**:
- **Database:** Eloquent, Doctrine, or raw DBAL (your choice).
- **Real-Time:** WebSockets, task manager, process pooling.
- **Auth:** JWT/OAuth2 out of the box.

*No bloat. Swap anything.*

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


![image](https://github.com/odysee-dev/.github/blob/master/profile/cover.png?raw=true)
# ODY framework

(🚀 Swoole-Powered, Async-First, and Laravel-Simple)

ODY is a lightweight high-performance asynchronous PHP framework designed for building microservices and RESTful APIs with ease. Built on top of Swoole, ODY leverages asynchronous processing and coroutines to deliver exceptional performance while maintaining a clean, developer-friendly architecture.

**Warning:**  
🔥 *"After using ODY, going back to Laravel feels like driving a tractor on the Autobahn."*  
*(Yes, it’s that fast. No, it’s not production-ready yet—but you’ll wish it was.)*

## **Why ODY Exists**
Laravel is **slow**. Node.js is **a mess**. Traditional PHP blocks like it’s 2004.

- **Node.js-like speed** (thanks to Swoole’s coroutines).
- **Laravel-like elegance** (PSR standards, clean APIs).
- **Zero JavaScript tax** (real-time apps without Node.js/Redis/Echo/npm modules bloat nonsense).

## 🚀 Key Features

- **High Performance**: Built with Swoole support for asynchronous processing and coroutines
- **PSR Compliance**: Implements PSR-7, PSR-15, and PSR-17 for HTTP messaging and middleware
- **Modular Design**: Build and integrate different modules
- **Middleware System**: Middleware system for request/response processing
- **Dependency Injection**: Built-in IoC container for dependency management
- **Console Support**: CLI commands for various tasks and application management
- **Routing**: Simple and flexible routing system with support for route groups and middleware

| **Feature**       | **ODY**                          | **Laravel**                     | **Node.js**               |  
|-------------------|----------------------------------|---------------------------------|---------------------------|  
| **WebSockets**    | Native PHP, 5-minute setup       | Requires Node.js + Echo + Redis | Native (but JavaScript 😩)|  
| **Async Tasks**   | Built-in, no queue workers       | Needs Redis + `supervisorctl`   | Callback hell             |  
| **Concurrency**   | 8K+ req/sec on a $5 VM         | 500 req/sec (if lucky)          | Fast but chaotic          |  
| **CQRS**         | Async/sync, 5-line config       | DIY + AMQP + pain               | 🤷‍♂️                      |  

## **📦 Batteries Included (But Modular)**
Need more? ODY ships with **13+ modules**:
- **Database:** Eloquent, Doctrine, or raw DBAL (your choice).
- **Real-Time:** WebSockets, task manager, process pooling.
- **DevOps:** InfluxDB metrics, connection pooling, caching.
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
- [X] 8K RPS benchmarks on lightweight machines 

**Dare to try it?**
```bash
composer create-project ody/framework ody && cd ody && php ody server:start  
```  

## Documentation

Visit [ody.dev/docs](https://ody.dev/docs) or dive into the packages on this GitHub account,
they contain a lot of information and API references that are not published on the official documentation yet.

## License

ODY Framework is open-source software licensed under the MIT license.


![image](https://github.com/odysee-dev/.github/blob/master/profile/cover.png?raw=true)
# ODY framework
ODY is a lightweight high-performance asynchronous PHP framework designed for building microservices and RESTful APIs with ease. Built on top of Swoole, ODY leverages asynchronous processing and coroutines to deliver exceptional performance while maintaining a clean, developer-friendly architecture.

> [!WARNING]
> 🚧 Not production-ready. ODY is actively being developed. There will be unexpected bugs.

## Key Features

- **High Performance**: Built with Swoole support for asynchronous processing and coroutines
- **PSR Compliance**: Implements PSR-7, PSR-15, and PSR-17 for HTTP messaging and middleware
- **Modular Design**: Build and integrate different modules
- **Middleware System**: Middleware system for request/response processing
- **Dependency Injection**: Built-in IoC container for dependency management
- **Console Support**: CLI commands for various tasks and application management
- **Routing**: Simple and flexible routing system with support for route groups and middleware

## Installation

Requires php8.3 or above.

Before installing the framework please make sure you have `php8.x-swoole` installed

```
composer create-project ody/framework ody
```

## Documentation

For (for now) incomplete documentation, visit [ody.dev/docs](https://ody.dev/docs) or dive into the packages on this GitHub account,
they contain a lot of information and API references that are not published on the official documentation yet.

## License

ODY Framework is open-source software licensed under the MIT license.


![image](https://github.com/odysee-dev/.github/blob/master/profile/cover.png?raw=true)
# ODY framework
ODY is a lightweight PHP coroutine framework designed for API development and microservices, built on top of Swoole’s powerful asynchronous capabilities. It keeps things minimal, allowing you to pick only what you need and integrate it your way.


> [!WARNING]
> 🚧 Not production-ready. ODY is actively being developed. While the core functionality is stable, additional components and features are continuously being added.

## Install a skeleton project
Installing ody-skel provides a basic framework with every component and their corresponding configuration files installed. In addition a couple of example classes line controllers, models, jobs and commanands in `app/` are provided to get you started right away.
At the moment it ships with Eloquent as ORM. You can run most of swoole's coroutine functionality in classes that go throught the request lifecycle. Try it out!

```
create-project ody/ody-skel ody 0.0.1

# Start a HTTP server
php ody server:start

curl 127.0.0.1:9501/users

# Start the scheduler (a example job that runs every minute gets scheduled)
php ody scheduler:start

# start a websocket server
php ody websocket:start
```



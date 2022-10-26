# graalvm-with-spring-native

Originally Chicago Java Users Group (CJUG), April 25, 2022

## Getting Started

1. Clone the repository
    ```shell
    git@github.com:dashaun/graalvm-with-spring-native.git
    ```
2. CD into the repository
    ```shell
    cd graalvm-with-spring-native
    ```
3. Install [vendir](https://carvel.dev/vendir/docs/v0.24.0/install)
4. Download reveal.js
   Setup:
    ```shell
    vendir sync
    ```
5. Use docker to serve the content
    ```shell
   ./mvnw spring-boot:run
    ``` 
6. Open browser to http://localhost:8080/

## Development

```shell
docker run --name seattle --rm -v $PWD/src/main/resources/static/:/usr/share/nginx/html:ro -d -p 8088:80 nginx
```
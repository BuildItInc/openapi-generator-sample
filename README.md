# OpenAPI-Generator sample

OpenAPI および、OpenAPI generatorをお試しするためのrepository。 

## Requirement

* Docker

## Usage

### Docker Service 起動

Terminalで、docker processを立ち上げる
```sh
docker-compose up -d
```

### ブラウザから各サービスへ

docker processが起動した後に、ブラウザで下記接続先にアクセスすることで、各サービスを利用できる。

|サービス名|接続先(port番号)|
|:---:|:---:|
|apisprout|localhost:8000|
|swagger-ui|localhost:8081|
|swagger-editor|localhost:8082|

### OpenAPI generator でのコード生成

```sh
docker-compose run openapi-generator generate -i swagger/api.yaml -g {language}
```

## Note

* [apisprout](https://github.com/danielgtaylor/apisprout)
* [swagger-ui](https://swagger.io/tools/swagger-ui/)
* [swagger-editor](https://editor.swagger.io/)
* [OpenAPI generator](https://github.com/OpenAPITools/openapi-generator)

# Duolingo Unofficial API Definition

![](https://github.com/igorskh/duolingo-api/workflows/Node.js%20CI/badge.svg)

## Description
Unofficial OpenAPI 2.0 (aka Swagger) definition for Duolingo API.

The validation and codegen was tested for Golang with [go-swagger](https://github.com/go-swagger/go-swagger).

## Validate and Generate Server/Client Code
Validate documentation:
```bash
# node.js swagger
npx swagger validate swagger.yaml
# go-swagger
swagger validate
```

Generate client:
```bash
swagger generate client -f ./duolingo-api/swagger.yaml
```

Generate server:
```bash
swagger generate server -f ./duolingo-api/swagger.yaml
```

See more documentation on [https://goswagger.io](https://goswagger.io).

Generate interactive documentation:
```bash
npx redoc-cli bundle swagger.yaml
```

## Mock Server with Prism
For mocking purpose [Prism](https://stoplight.io/open-source/prism/) is used.

```
npx prism mock swagger.yaml
```

## Implementations
* [Golang](https://github.com/igorskh/go-duolingo)

# Setup

```sh
go get github.com/graphql-go/graphql
```


# Examples

## Example 1
Very basic example, is a 'hello world'

## Example 2
Is a more complex example, graphql with structs

## Example 3
Is an application web with graphQL without any external packages (without gorilla mux and gin)


## gplgen
repo: https://github.com/99designs/gqlgen
```sh
mkdir example
cd example
go mod init example

printf '// +build tools\npackage tools\nimport _ "github.com/99designs/gqlgen"' | gofmt > tools.go
go mod tidy

go run github.com/99designs/gqlgen init

go run server.go
```
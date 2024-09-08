##Simulation of three body problem

As title says, this is a try to create an simulation of three body problem in Golang. Choosing of go here is trival, because the reason is a learning experience.
To make it available via website, as a middle-man WebAssembly is used.

#### How to run it locally

1. You need to have go installed on your machine.
2. Install all dependencies by using `go mod tidy`
3. Set up env variables

```sh
set GOARCH=wasm
set GOOS=js
```

4. Build WASM

```sh
go build -o main.wasm
```

5. Serve it. I'm using python http server. `python3 -m http.server`

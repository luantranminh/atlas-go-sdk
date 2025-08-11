# Atlas SDK for Go

> [!NOTE]
> This repostiroy has been archived. Use [ariga.io/atlas/atlasexec](https://github.com/ariga/atlas) instead.

[![Go Reference](https://pkg.go.dev/badge/github.com/luantranminh/atlas-go-sdk/atlasexec.svg)](https://pkg.go.dev/github.com/luantranminh/atlas-go-sdk/atlasexec)

An SDK for building ariga/atlas providers in Go.

## Installation

```bash
go get -u github.com/luantranminh/atlas-go-sdk
```

## How to use

To use the SDK, you need to create a new client with your `migrations` folder and the `atlas` binary path.

```go
package main

import (
    ...
    "github.com/luantranminh/atlas-go-sdk/atlasexec"
)

func main() {
    // Create a new client
    client, err := atlasexec.NewClient("my-migration-folder", "my-atlas-cli-path")
    if err != nil {
        log.Fatalf("failed to create client: %v", err)
    }
}
```

## APIs

For more information, refer to the documentation available at [GoDoc](https://pkg.go.dev/github.com/luantranminh/atlas-go-sdk/atlasexec#Client)

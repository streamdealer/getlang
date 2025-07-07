# getlang

[![GoDoc](https://godoc.org/github.com/streamdealer/getlang?status.svg)](https://godoc.org/github.com/streamdealer/getlang) [![Go Report Card](https://goreportcard.com/badge/github.com/streamdealer/getlang)](https://goreportcard.com/report/github.com/streamdealer/getlang) [![Build Status](https://travis-ci.org/streamdealer/getlang.svg?branch=master)](https://travis-ci.org/streamdealer/getlang) ![cover.run go](https://cover.run/go/github.com/streamdealer/getlang.svg?tag=golang-1.10)

getlang provides fast natural language detection in Go.

## Features

* Offline -- no internet connection required
* Supports [30 languages](https://github.com/streamdealer/getlang/blob/master/LANGUAGES.md)
* Provides ISO 639 language codes
* Fast

## Getting started

Installation:
```sh
    go get -u github.com/streamdealer/getlang
```

example:
```go
package main

import (
	"fmt"
	"github.com/streamdealer/getlang"
)

func main(){
  info := getlang.FromString("Wszyscy ludzie rodzą się wolni i równi w swojej godności i prawach")
  fmt.Println(info.LanguageCode(), info.Confidence())
}
```

## License
[MIT](https://github.com/streamdealer/getlang/blob/master/LICENSE)

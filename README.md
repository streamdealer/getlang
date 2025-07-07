# getlang

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

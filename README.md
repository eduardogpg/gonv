# Gonv

This is a library with which you can get environment variables in a very simple way, you can get session variables of different values.

  - String
  - Int
  - Boolean

> If the environmental variable does not exist in the computer you can pass a default value. You can create the enviromental variable wiht GetEnvOrCreate function.
s
### Installation

```sh
 go get -u github.com/eduardogpg/gonv
```

### Examples

Simple example with String, int and boolean type.

```sh
package main

import(
  "fmt"
  "github.com/eduardogpg/gonv"
)

func main() {
      
    host := gonv.GetStringEnv("HOST", "localhost")
    port := gonv.GetIntEnv("PORT", 8000)
    debug := gonv.GetBoolEnv("DEBUG", false)

    fmt.Println(host)
    fmt.Println(port)
    fmt.Println(debug)
}

```

### Developer
@eduardo_gpg

License
----

MIT


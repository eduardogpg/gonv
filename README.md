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

func init(){

}

func main(){
  host := gonv.GetStringEnv("HOST", "localhost")
  port := gonv.GetIntEnv("PORT", 3306)
  debug := gonv.GetBoolEnv("DEBUG", false)

  final := fmt.Sprintf("%s:%d debug mode : %t", host, port, debug)
  fmt.Println(final)
}

```

### Developer
@eduardo_gpg

License
----

MIT

  
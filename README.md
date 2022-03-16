# shukujitsu

[![PkgGoDev](https://pkg.go.dev/badge/github.com/soh335/shukujitsu)](https://pkg.go.dev/github.com/soh335/shukujitsu) ![test](https://github.com/soh335/shukujitsu/workflows/test/badge.svg)

shukujitsu determines japanese holiday.
Holidays are collected from https://www8.cao.go.jp/chosei/shukujitsu/syukujitsu.csv

When csv is updated, you can updated as follow command.

```
$ go run ./internal/gen/gen.go
```

Currently, we check it per week at [here](https://github.com/soh335/shukujitsu/actions?query=workflow%3Aupdate).

## HOW TO USE

```go
if shukujitsu.IsShukujitsu(time.Now()) {
    fmt.Println("shukujitsu!")
}
```


## MEMO(kenall)
https://twitter.com/kenalljp/status/1503884558105989120
https://blog.kenall.jp/entry/japan-holiday-api-release

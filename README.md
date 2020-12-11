# github.com/qiniu/stack-go (七牛云主机服务 Go SDK)

[![LICENSE](https://img.shields.io/github/license/qiniu/api.v7.svg)](https://github.com/qiniu/stack-go/blob/master/LICENSE)
[![Build Status](https://travis-ci.org/qiniu/stack-go.svg?branch=master)](https://travis-ci.org/qiniu/stack-go)

[![Qiniu Logo](http://open.qiniudn.com/logo.png)](http://qiniu.com/)

## Installation

```
go get github.com/qiniu/stack-go
```

## Examples

```golang
import (
  ...
  "github.com/qiniu/stack-go"
)

func main() {
  s := stack.New(logger.New(), "https://api-qvm.qiniu.com", auth.auth.NewCredential("xxx", "xxx"))

  resp, _ := s.ECS().ListInstances(&ecs.ListInstancesParams{...})

  ...
}
```

## License

stack-go is released under the Apache 2.0 license. See [LICENSE.txt](https://github.com/qiniu/stack-go/blob/master/LICENSE)

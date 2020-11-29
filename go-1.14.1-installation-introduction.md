# Go 1.14.1安装和使用

- ### 安装

从[https://studygolang.com/dl](https://studygolang.com/dl)下载最新稳定版本go1.14.1.linux-amd64.tar.gz。上传到CentOS。

解压开，并移到/usr/local/目录下。

    tar zxvf go1.14.1.linux-amd64.tar.gz
    mv go /usr/local/

配置Go的环境变量。

    vi /etc/profile
    export GOROOT=/usr/local/go
    export GOPATH=/root/go
    export GO111MODULE="on"
    export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
    
    source /etc/profile

查看Go版本和环境变量

    go version
    go version go1.14.1 linux/amd64
    
    go env
    GO111MODULE="on"
    GOARCH="amd64"
    GOBIN=""
    GOCACHE="/root/.cache/go-build"
    GOENV="/root/.config/go/env"
    GOEXE=""
    GOFLAGS=""
    GOHOSTARCH="amd64"
    GOHOSTOS="linux"
    GOINSECURE=""
    GONOPROXY=""
    GONOSUMDB=""
    GOOS="linux"
    GOPATH="/root/go"
    GOPRIVATE=""
    GOPROXY="https://proxy.golang.org,direct"
    GOROOT="/usr/local/go"
    GOSUMDB="sum.golang.org"
    GOTMPDIR=""
    GOTOOLDIR="/usr/local/go/pkg/tool/linux_amd64"
    GCCGO="gccgo"
    AR="ar"
    CC="gcc"
    CXX="g++"
    CGO_ENABLED="1"
    GOMOD="/dev/null"
    CGO_CFLAGS="-g -O2"
    CGO_CPPFLAGS=""
    CGO_CXXFLAGS="-g -O2"
    CGO_FFLAGS="-g -O2"
    CGO_LDFLAGS="-g -O2"
    PKG_CONFIG="pkg-config"
    GOGCCFLAGS="-fPIC -m64 -pthread -fmessage-length=0 -fdebug-prefix-map=/tmp/go-build845031564=/tmp/go-build -gno-record-gcc-switches"












# Stook-S3-benchmark

# Linux:
```bash
apt-get update
apt-get install git golang
mkdir $HOME/work
cd $HOME/work
git clone https://github.com/chinglinwen/s3-benchmark.git
export GOPATH=$HOME/work
export GOROOT=/usr/lib/go
go get code.cloudfoundry.org/bytefmt
go get github.com/aws/aws-sdk-go
cd $HOME/s3-benchmark
go build s3-benchmark.go
```
# MacOS: 
```bash
GOOS=darwin GOARCH=amd64 go build s3-benchmark.go
```
# Windows
```bash
GOOS=windows GOARCH=amd64 go build s3-benchmark.go
```

# Use
```bash
./s3-benchmark -u https://xxxxx.mncdn.com -a yyyyyyyyy -b test -s zzzzzzzzz -t 10
```

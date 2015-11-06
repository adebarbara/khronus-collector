khronus-collector
=======

## Install
```bash
git clone https://github.com/Searchlight/khronus-collector.git
egrep -rho '(github.*)[^\"]' * | sort -u | xargs -P1 -L1 go get -u
go build -o bin/khronus-collector src/khronus-collector.go
```

## Run
```bash 
export DEFAULT_CONFIG=$(./bin/khronus-collector --show-config)
./bin/khronus-collector --config="${DEFAULT_CONFIG}"
```

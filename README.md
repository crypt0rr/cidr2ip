# cidr2ip

This program converts IPv4 CIDR blocks into their constituent IP addresses.

## Input modes

1. Commnd line arguments

```plain
$ cidr2ip 10.0.0.0/30 192.68.0.0/30
10.0.0.1
10.0.0.2
192.68.0.1
192.68.0.2
```

2. Piped input

```plain
$ cat cidrs.txt | cidr2ip
192.168.0.101
192.168.0.102
```

3. File input

```plain
$ cidr2ip -f cidrs.txt
192.168.0.101
192.168.0.102
```

### Install

#### Download from the releases pages

Download pre-built binary from the release page.

```plain

```

#### Use `go install`

If you have `golang` tools installed, you can download and build the source code locally as follows:

```plain
go install github.com/crypt0rr/cidr2ip@latest
```

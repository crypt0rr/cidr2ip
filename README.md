# cidr2ip

This program converts IPv4 CIDR blocks into their constituent IP addresses.

## Install

```plain
go install github.com/crypt0rr/cidr2ip@latest
```

## Usage

### 1. Command line arguments

It is possible to use one or more CLI arguments.

```plain
$ cidr2ip 10.0.0.0/30 192.68.0.0/30
10.0.0.1
10.0.0.2
192.68.0.1
192.68.0.2
```

### 2. Piped input

Pipe a file containing networks (e.g. `192.168.0.100/30`) to `cidr2ip`

```plain
$ cat cidrs.txt | cidr2ip
192.168.0.101
192.168.0.102
```

### 3. File input

Instead of piping the content of a file to `cidr2ip` it can also be used directly.

```plain
$ cidr2ip -f cidrs.txt
192.168.0.101
192.168.0.102
```

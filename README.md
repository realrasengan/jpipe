# jpipe
## Run JS from the cmdline or with pipe
### Inspired by [pyp](https://github.com/hauntsaninja/pyp)

### Installation
```
git clone https://github.com/realrasengan/jpipe
cd jpipe
```

Then, copy "jpipe" to a folder in your PATH or add this folder to your PATH.

### Usage Examples

Run simple JS
```
./jpipe "console.log('Hello World')"
```

Get load from uptime (I know it's in /proc/)
```
uptime | ./jpipe "console.log(buffer.split(': ')[1])"
```

Parse a JSON (I know you can use jq)
```
cat test.json | ./jpipe "console.log(JSON.parse(buffer).name)"
```
test.json included in this repo.

### License and Copyright

Copyright (C) 2020 Andrew Lee <andrew@imperialfamily.com>

MIT Licensed

# nodejs-caeser-cipher-cli

A simple NodeJS CLI tool to encode and decode a string by [Caesar cipher](https://en.wikipedia.org/wiki/Caesar_cipher)

## Installation

Before you run CLI tool, please, run this command:
```
npm install
```

CLI accepts 4 options (short alias and full name):

1.  **-s, --shift**: a shift
2.  **-i, --input**: an input file
3.  **-o, --output**: an output file
4.  **-a, --action**: an action encode/decode

**Usage example:**

```bash
$ node my_caesar_cli -a encode -s 7 -i "./input.txt" -o "./output.txt"
```

```bash
$ node my_caesar_cli --action encode --shift 7 --input plain.txt --output encoded.txt
```

```bash
$ node my_caesar_cli --action decode --shift 7 --input decoded.txt --output plain.txt
```

> input.txt
> `This is secret. Message about "_" symbol!`

> output.txt
> `Aopz pz zljyla. Tlzzhnl hivba "_" zftivs!`

!!!! It searches for input file starting from the same level as `caeser-cipher-cli` folder.
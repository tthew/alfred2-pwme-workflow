# Alfred2 'pwme' workflow

> Alfred2 workflow wrapper for `pwgen`

Generate secure random passwords using pwgen and copy to the clipboard.

## Prerequisites / installation

`pwme` depends on `pwgen` and expects `pwgen` binary to be available at `/usr/local/bin/pwgen`

`pwgen` is available as a Homebrew package, to install simply run:

```bash
brew install pwgen
```

## Usage

`pwme {numberOfChars}`

{numberOfCharacters} is optional, defaults to 8 if omitted.

### Under the hood

Calls pwgen with the following arguments:

```bash
pwgen -cnysB1
```

## License

Apache-2

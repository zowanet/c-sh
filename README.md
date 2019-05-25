# c

Invokes your C compiler's preprocessor allowing you to query for the preprocessed result of any symbol.

Supports all of the following, provided the relevant header files are found on your machine in `/usr/include/`:

* C Standard Library
* POSIX Standard Library
* BSD Standard Library

## Installation

Clone this repository, then run `./install`.
The script will be symlinked into your `~/bin/` directory.

To update, run `git fetch origin && git pull origin master`.

## Usage

```bash
c
```
> Outputs
>
>     Usage: c SYMBOL

## Examples

```bash
c PATH_MAX
```
> Outputs
>
>     1024

```bash
c AF_INET6
```
> Outputs
>
>     30

```bash
c PRIu64
```
> Outputs
>
>     "ll" "u"


# README.md example


<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

  - [About](#about)
  - [Features](#features)
  - [Requirements](#requirements)
    - [Runtime](#runtime)
    - [Development](#development)
  - [Install](#install)
    - [Download](#download)
    - [Installation](#installation)
  - [Freqlenty asked Questions](#freqlenty-asked-questions)
  - [History](#history)
  - [Links](#links)
  - [Contribute](#contribute)
  - [License](#license)
- [Some examples, remove after creation](#some-examples-remove-after-creation)
- [The largest heading](#the-largest-heading)
  - [The second largest heading](#the-second-largest-heading)
          - [The smallest heading](#the-smallest-heading)
  - [Text styles](#text-styles)
  - [Tables](#tables)
  - [List](#list)
  - [Task list](#task-list)
  - [Code Highlight](#code-highlight)
  - [Colapsed section](#colapsed-section)
    - [We can hide anything, even code!](#we-can-hide-anything-even-code)
  - [Links](#links-1)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## About


## Features


## Requirements

### Runtime

### Development


## Install

### Download

### Installation


## Freqlenty asked Questions


## History 

[HISTORY.md](/HISTORY.md)


## Links


## Contribute


## License 


# Some examples, remove after creation

# The largest heading
## The second largest heading
###### The smallest heading


`quoting code`

```c
void main(int arc, char argv**) {
  exit 0;
}
```

## Text styles

| Style  | Syntax  | Example | Output |
|------- |-------- |---------|--------|
| Bold   | `** **` | `**This is bold text**`  | **This is bold text** |
| Italic | `* *`   | ` *This text is italicized*` | *This text is italicized* |
| Strikethrough | `~~ ~~` | `~~This was mistaken text~~` | ~~This was mistaken text~~ |
| Subscript | `<sub> </sub>` | `Ordinary, <sup>subscript</sub>` | Ordinary <sub>subscript</sub> |
| Superscript | `<sup> </sup>` | `Ordinary, <sup>superscript</sup>` | Ordinary <sup>superscript</sup> |

> Text that is a quote

## Tables

| Header 1 | Header 2 |
| -------- | -------- |
|   C1     | C2       |
|   C3     | C4       |


## List

- Item 1
- Item 2
- Item 3

## Task list

- [ ] Task 1
- [x] Task 2
- [ ] Task 3


## Code Highlight

```c 
#include <stdio.h>

int main(int argc, char *argv[]) {
  int error;

  // --- Command line arguments ---
  //---------------------------------------------------------------------------
  struct arg_lit *help     = arg_lit0("h",  "help",                  "Show help");
  struct arg_lit *version  = arg_lit0(NULL, "version",               "Version");
  struct arg_lit *verbose  = arg_lit0("v",  "verbose",               "Verbose output");
  struct arg_end *end      = arg_end(20);

  void *argtable[] = { help, version, verbose, end};

  // Print helptext
  if (help->count) {
    arg_print_glossary(stdout,argtable,"  %-30s %s\n");
    exit(0);
  }

  printf("Ett litet testprogram.\n");

  lua_State *L = luaL_newstate();
  luaL_openlibs(L);
  luaL_dofile(L, "test.lua");

  return 0;
}
```

```python
def kalle():
  print("Nisse")
  x = 23
```

```c
#include <stdio.h>

void main(int a) {
  printf("Kalle\n");
  return 0;
}
```


## Colapsed section

<details><summary>CLICK ME</summary>
<p>

### We can hide anything, even code!

```ruby
puts "Hello World"
```

</p>
</details>

## Links

[Markup basics](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls)

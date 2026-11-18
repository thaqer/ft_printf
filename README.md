# ft_printf

A 42 Amman project that re-implements `printf`. It returns the number of characters printed, like the real one.

## Supported conversions

| Conversion | Prints |
| --- | --- |
| `%c` | a character |
| `%s` | a string (`(null)` for `NULL`) |
| `%p` | a pointer in hex, e.g. `0x1234` |
| `%d` `%i` | a signed decimal integer |
| `%u` | an unsigned decimal integer |
| `%x` `%X` | an unsigned integer in lowercase / uppercase hex |
| `%%` | a literal `%` |

Flags, field width and precision are not supported.

## Build

```sh
make            # builds libftprintf.a
cc main.c -I. libftprintf.a
```

```c
#include "ft_printf.h"

int main(void)
{
	ft_printf("%s is %d years old, %x in hex\n", "libft", 2, 255);
	return (0);
}
```

## Author

[thaqer](https://github.com/thaqer), 42 Amman.

```
#include <string.h>
void *memchr(const void *s, int c, size_t n);
```
DESCRIPTION:
	`The memchr() scans n bytes of the memory area pointed to by s for the first instance of c. Both c and the bytes of the memory area pointed to by s are interpreted as unsigned char.`

RETURN VALUE:
	Return a pointer to the matching byte or NULL if the character does not occur in the given memory area.

#memory #scanning #libft

```NOTES 

``` 

```EDGE_CASES
// n == 0
will return `NULL`
// c == '\0'
will return its memory address if it falls within the $n$ limit
// Values outside the 0-255 range are truncated 
```
SRC: https://github.com/lattera/glibc/blob/master/string/memchr.c
MAN: https://man.archlinux.org/man/memchr.3
```
#include <string.h>
void *memrchr(const void *s, int c, size_t n);
```
DESCRIPTION:	
`The memrchr() function is like the memchr() function, except that it searches backward from the end of the n bytes pointed to by s instead of forward from the beginning.`

RETURN VALUE:
Returns a pointer to the matching byte or NULL if the character does not occur in the given memory area. 

#memory #scanning #libft

```NOTES 
// Typecast staff
// Scan backward up to n bytes
// If a match is found, return a pointer to that specific byte
// Return NULL if n bytes are scanned without a match
``` 

```EDGE_CASES
// n == 0
will return NULL
// c == '\0'
will return its memory address if it falls within the $n$ limit
// Values outside the 0-255 for `int c` range are truncated 
will be casted to unsigned char == (0-255)
// Target found beyond n bound 
will return NULL
```
SRC: https://github.com/lattera/glibc/blob/master/string/memrchr.c
MAN: https://man.archlinux.org/man/memrchr.3
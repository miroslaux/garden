```
#include <strings.h.>
void bzero(void *s, size_t n);
```
DESCRIPTION:	
`The bzero() function erases the data in the n bytes of the memory starting at the location pointed to by s, by writing zeros (bytes containing '\0') to that area.`

RETURN VALUE:
None.

#setting #zero #memory #libft

```NOTES 
simply: just memset with 0's.

// Why we are able to ignore return value of memset ?

C allows to ignore any function's return value, bzero lets memset do the work and safely discards the pointer memset returns.
``` 

```EDGE_CASES
// n == 0
char buffer[10] = "Hello";
bzero(buffer, 0); 

// offset value 
char array[10] = "123456789";
bzero(array + 5, 3);

// uninitialized, just allocated memory
char *ptr = malloc(100);
bzero(ptr, 100);
```
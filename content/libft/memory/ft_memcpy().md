```
#include <string.h>
void *memcpy(void *dest, const void *src, size_t n);
```
DESCRIPTION:

`The memcpy() function copies n bytes from memory area src to memory area dest. The memory areas must not overlap. Use memmove() if the memory areas do overlap.`

RETURN VALUE:

The memcpy() function returns a pointer to dest.

#memory #copy #libft

```NOTES 
overlap example: 
memcpy(p+1, p, 42); - undefined behaviour. 
memmove()
``` 

```EDGE_CASES
// copying src to dest when it's the same 
char buffer[10] = "0123456789";
memcpy(buffer, buffer, 10)

// n == 0
memcpy(dest, src, 0)

// Allocated, but contains random garbage
char *src = malloc(10);  
char dest[10];
memcpy(dest, src, 10);

// Shift data forward
char *src = &buffer[3];  // "3456789"
char *dest = &buffer[0]; // "0123..."
memcpy(dest, src, 5); 

```
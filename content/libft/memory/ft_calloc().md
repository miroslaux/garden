```
#include <stdlib.h>
void *calloc(size_t n, size_t size);
```
DESCRIPTION:
	`The calloc() function allocates memory for an array of n elements of size bytes each and returns a pointer to the allocated memory. The memory is set to zero. If n or size is 0, then calloc() returns a unique pointer value that can later be successfully passed to free()`

`free() `
	`The free() function frees the memory space pointed to by p, which must have been returned by a previous call to malloc() or related functions. Otherwise, or if p has already been freed, undefined behavior occurs. If p is NULL, no operation is performed.`

RETURN VALUE:
	Return a pointer to the allocated memory, which is suitably aligned for any type that fits into the requested size or less. On error, these functions return NULL. 

#setting #memory #libft

```NOTES 
//Prevent integer overflow during multiplication
//If count or size is 0, standard calloc returns a unique pointer that can be freed. 
//Allocate memory 
//Initialize the entire allocated memory block to zero
``` 

```EDGE_CASES
// count == 0 or size == 0

// integer overflow 
If `count * size` exceeds the maximum value of `size_t` - it will return NULL. 
```
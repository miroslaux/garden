```
#include <string.h>
int memcmp(const void *s1, const void *s2, size_t n);
```
DESCRIPTION:	
`The memcmp() function compares the first n bytes (each interpreted as unsigned char) of the memory areas s1 and s2.`

RETURN VALUE:
The memcmp() function returns an integer less than, equal to, or greater than zero if the first n bytes of s1 is found, respectively, to be less than, to match, or be greater than the first n bytes of s2. For a nonzero return value, the sign is determined by the sign of the difference between the first pair of bytes (interpreted as unsigned char) that differ in s1 and s2. If n is zero, the return value is zero.

#compare #memory #libft

```NOTES 
converting both memory areas to set's of pointers of unsigned chars and then
returning difference or 0 if it's equal
``` 

```EDGE_CASES
//  n == 0
memcmp(s1, s2, 0);

// signed vs unsigned 
char s1[] = {0xFF}; // -1 if signed
char s2[] = {0x01}; //  1 if signed
ft_memcmp(s1, s2, 1); 

// overlapping
char arr[] = "aaaa";
ft_memcmp(arr, arr + 1, 2);
```
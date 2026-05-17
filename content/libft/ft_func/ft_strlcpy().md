```
#include <string.h>
size_t strlcpy(char *dst, const char *src, size_t size);
```

DESCRIPTION:	
`The strlcpy() function copies up to size - 1 characters from the NUL-terminated string src to dst, NUL-terminating the result.`

The [[ft_strlcpy()]] - copy,  [[ft_strlcat()]] - concatenate C strings. Both designed to be safer, more consistent, and less error prone replacements for [[ft_strncpy()]] & [[ft_strncat()]]. Unlike N's, L's take the full size of the buffer (not just the length) and guarantee to NUL-terminate the result (as long as size is larger than 0 or, in the case of [[ft_strlcat()]], as long as there is at least one byte free in dst). 
- Byte for the NUL should be included in size. 
- Both only operate on true "C" strings -
- src must be NUL-terminated for [[ft_strlcpy]]

RETURN VALUE:
Both [[strlcpy()]] and [[strlcat()]] functions return the total length of the string they tried to create. For [[strlcpy()]] that means the length of src. For [[strlcat()]] that means the initial length of dst plus the length of src.  While this may seem somewhat confusing, it was done to make
truncation detection simple. Note, however, that if [[strlcat()]] traverses size characters without finding a NUL, the length of the string is considered to be size and the destination string will not be NUL-terminated (since there was no space for the NUL). This keeps [[strlcat()]] from running off the end of a string. In practice this should not happen (as it means that either size is incorrect or that dst is not a proper "C" string). The check exists to prevent potential security problems in incorrect code.

#copy #string #libft

```NOTES 

``` 

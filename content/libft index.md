
| [[ft_strlen]]  | ```size_t strlen(const char s);```                         |
| :------------- | :--------------------------------------------------------- |
| [[ft_memcpy]]  | ```void *memcpy(void *dest, const void *src, size_t n);``` |
| [[ft_memset]]  | ```void *memset(void *s, int c, size_t n);```              |
| [[ft_bzero]]   | ```void bzero(void *s, size_t n);```                       |
| [[ft_memmove]] | Copies memory area (safe for overlapping regions)          |
| [[ft_memcmp]]  | Compares memory areas                                      |
| [[ft_memchr]]  | Scans memory for a character                               |

| [[ft_isalpha]] | Checks for an alphabetic character.                   |
| :------------- | :---------------------------------------------------- |
| [[ft_isdigit]] | Checks for a digit (0 through 9).                     |
| [[ft_isalnum]] | Checks for an alphanumeric character.                 |
| [[ft_isascii]] | Checks whether `c` fits into the ASCII character set. |
| [[ft_isprint]] | Checks for any printable character.                   |

| [[ft_toupper]] | Converts a lower-case letter to upper case.                       |
| :------------- | :---------------------------------------------------------------- |
| [[ft_tolower]] | Converts an upper-case letter to lower case.                      |
| [[ft_strchr]]  | Locates the first occurrence of a character in a string[cite: 1]. |
| [[ft_strrchr]] | Locates the last occurrence of a character in a string[cite: 1].  |

| [[ft_strlcat]] | Size-bounded string concatenation[cite: 1].                                   |
| :------------- | :---------------------------------------------------------------------------- |
| [[ft_strlcpy]] | Size-bounded string copying[cite: 1].                                         |
| [[ft_atoi]]    | Converts a string to an integer[cite: 1].                                     |
| [[ft_strnstr]] | Locates a substring in a string, searching at most `len` characters[cite: 1]. |
| [[ft_strncmp]] | Compares two strings up to `n` characters[cite: 1].                           |
| [[ft_calloc]]  | Allocates memory and initializes it to zero                                   |
| [[ft_strdup]]  | Creates a duplicate of a string                                               |

| [[ft_substr]]   | Extracts a substring from a string[cite: 1].                                      |
| :-------------- | :-------------------------------------------------------------------------------- |
| [[ft_strjoin]]  | Concatenates two strings into a new one[cite: 1].                                 |
| [[ft_strtrim]]  | Trims specified characters from the beginning and end of a string[cite: 1].       |
| [[ft_split]]    | Splits a string into an array of strings using a delimiter[cite: 1].              |
| [[ft_itoa]]     | Converts an integer to a string[cite: 1].                                         |
| [[ft_strmapi]]  | Applies a function to each character of a string to create a new string[cite: 1]. |
| [[ft_striteri]] | Applies a function to each character of a string (in-place)[cite: 1].             |

| [[ft_putchar_fd]] | Outputs a character to the given file descriptor[cite: 1].                    |
| :---------------- | :---------------------------------------------------------------------------- |
| [[ft_putstr_fd]]  | Outputs a string to the given file descriptor[cite: 1].                       |
| [[ft_putendl_fd]] | Outputs a string followed by a newline to the given file descriptor[cite: 1]. |
| [[ft_putnbr_fd]]  | Outputs an integer to the given file descriptor[cite: 1].                     |
```c
typedef struct s_list
{
    void            *content;
    struct s_list   *next;
} t_list;
```

| [[ft_lstnew]]       | Creates a new list element.                                                |
| :------------------ | :------------------------------------------------------------------------- |
| [[ft_lstadd_front]] | Adds an element at the beginning of the list                               |
| [[ft_lstsize]]      | Counts the number of elements in the list                                  |
| [[ft_lstlast]]      | Returns the last element of the list.                                      |
| [[ft_lstadd_back]]  | Deletes an element and frees its content using a given function            |
| [[ft_lstadd_back]]  | Deletes and frees a list and its successors.                               |
| [[ft_lstiter]]      | Iterates over a list and applies a function to the content of each element |
| [[ft_lstmap]]       | Iterates over a list and applies a function to create a new list           |

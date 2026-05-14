
|                |                                                                   |
| :------------- | :---------------------------------------------------------------- |
| [[ft_strlen]]  | ```size_t strlen(const char s);```                                |
| [[ft_memcpy]]  | ```void *memcpy(void *dest, const void *src, size_t n);```        |
| [[ft_memset]]  | ```void *memset(void *s, int c, size_t n);```                     |
| [[ft_bzero]]   | ```void bzero(void *s, size_t n);```                              |
| [[ft_memmove]] | ```void *ft_memmove(void *dest, const void *src, size_t n);```    |
| [[ft_memcmp]]  | ```size_t ft_memcmp(const void *s1, const void *s2, size_t n);``` |
| [[ft_memchr]]  | ```void *ft_memchr(const void *s, int c, size_t n);```            |


|                |                              |
| :------------- | :--------------------------- |
| [[ft_isalpha]] | ```int ft_isalpha(int c);``` |
| [[ft_isdigit]] | ```int ft_isdigit(int c);``` |
| [[ft_isalnum]] | ```int ft_isalnum(int c);``` |
| [[ft_isascii]] | ```int ft_isascii(int c);``` |
| [[ft_isprint]] | ```int ft_isprint(int c);``` |

|                |                                               |
| :------------- | :-------------------------------------------- |
| [[ft_toupper]] | ```int ft_toupper(int c);```                  |
| [[ft_tolower]] | ```int ft_tolower(int c);```                  |
| [[ft_strchr]]  | ```char *ft_strchr(const char *s, int c);```  |
| [[ft_strrchr]] | ```char *ft_strrchr(const char *s, int c);``` |

|                |                                                                          |
| :------------- | :----------------------------------------------------------------------- |
| [[ft_strlcat]] | ```size_t ft_strlcat(char *dst, const char *src, size_t size);```        |
| [[ft_strlcpy]] | ```size_t ft_strlcpy(char *dst, const char *src, size_t size);```        |
| [[ft_atoi]]    | ```int ft_atoi(const char *nptr);```                                     |
| [[ft_strnstr]] | ```char *ft_strnstr(const char *big, const char *little, size_t len);``` |
| [[ft_strncmp]] | ```int ft_strncmp(const char *s1, const char *s2, size_t n);```          |
| [[ft_calloc]]  | ```void *ft_calloc(size_t n, size_t size);```                            |
| [[ft_strdup]]  | ```char *ft_strdup(const char *s);```                                    |

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

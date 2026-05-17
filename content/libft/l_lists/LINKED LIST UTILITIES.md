
```c
typedef struct s_list
{
    void            *content;
    struct s_list   *next;
} t_list;
```

| f()                   | [[LINKED LIST UTILITIES]]                                                      |
| :-------------------- | :----------------------------------------------------------------------------- |
| [[ft_lstnew()]]       | ```t_list *ft_lstnew(void *content);```                                        |
| [[ft_lstadd_front()]] | ```void ft_lstadd_front(t_list **lst, t_list *new);```                         |
| [[ft_lstsize()]]      | ```int ft_lstsize(t_list *lst);```                                             |
| [[ft_lstlast()]]      | ```t_list *ft_lstlast(t_list *lst);```                                         |
| [[ft_lstadd_back()]]  | ```void ft_lstadd_back(t_list **lst, t_list *new);```                          |
| [[ft_lstdelone()]]    | ```void ft_lstdelone(t_list *lst, void (*del)(void *));```                     |
| [[ft_lstclear()]]     | ```void ft_lstclear(t_list **lst, void (*del)(void *));```                     |
| [[ft_lstiter()]]      | ```void ft_lstiter(t_list *lst, void (*f)(void *));```                         |
| [[ft_lstmap()]]       | ```t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));``` |

![libft](https://user-images.githubusercontent.com/103765789/168682988-b193a664-22e7-4751-ad12-620adca7d073.JPG)

# Libft
Libft is the very first individual project at School21. It's goal is to recode a few functioins from C standart library and some extra functions. It's goal is to create a library that we'll be able to use in our future projects as we are not allowed to use standart libraries. Also. it helps us to understand the basic algorithms.
## Functions
| Mandatory | Additional | Bonus |
|---|---|---|
|[ft_atoi](#ft_atoi)|[ft_itoa](#ft_itoa) | [ft_lstadd_back](#ft_lstadd_back)
|[ft_bzero](#ft_bzero) | [ft_putchar_fd](#ft_putchar_fd) |[ft_lstadd_front](#ft_lstadd_front)
|[ft_calloc](#ft_calloc) | [ft_putendl_fd](#ft_putendl_fd) | [ft_lstclear](#ft_lstclear)
|[ft_isalnum](#ft_isalnum) | [ft_putnbr_fd](#ft_putnbr_fd) | [ft_lstdelone](#ft_lstdelone)
|[ft_isalpha](#ft_isalpha) | [ft_putstr_fd](#ft_putstr_fd) | [ft_lstiter](#ft_lstiter)
|[ft_isascii](#ft_isascii) |[ft_split](#ft_split)| [ft_lstlast](#ft_lstlast)
|[ft_isdigit](#ft_isdigit) | [ft_striteri](#ft_striteri) |[ft_lstmap](#ft_lstmap)
|[ft_isprint](#ft_isprint) | [ft_strjoin](#ft_strjoin) |[ft_lstnew](#ft_lstnew)
|[ft_memchr](#ft_memchr) | [ft_strmapi](#ft_strmapi) | [ft_lstsize](#ft_lstsize)
|[ft_memcmp](#ft_memcmp) | [ft_strtrim](#ft_strtrim) 
|[ft_memcpy](#ft_memcpy) | [ft_substr](#ft_substr)
|[ft_memmove](#ft_memmove) 
|[ft_memset](#ft_memset) 
|[ft_strchr](#ft_strchr)
|[ft_strdup](#ft_strdup)
|[ft_strlcat](#ft_strlcat)
|[ft_strlcpy](#ft_strlcpy)
|[ft_strlen](#ft_strlen)
| [ft_strncmp](#ft_strncmp)
| [ft_strnstr](#ft_strnstr)
| [ft_strrchr](#ft_strrchr)
|[ft_tolower](#ft_tolower)
| [ft_toupper](#ft_toupper)
____
## Description
### Mandatory
#### ft_atoi
```
int atoi (const char *str);
```
|Description | Parameters | Return Value|
|---|---|---|
|Convert string to integer | C-string needed to convert | Converted value|

#### ft_bzero
```
void	ft_bzero(void *s, size_t n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Writes first n-bytes as '\0' in s | s - string to operate with; n - bumber of bytes | ---|
#### ft_calloc
```
void* calloc (size_t num, size_t size);
```
|Description | Parameters | Return Value|
|---|---|---|
|Allocates a block of memory for an array of *num* elements, each of them *size* bytes long, and initializes all its bits to zero. | *num* - number of elements; *size* - size of bytes | A pointer to the memory block allocated by the function.|
#### ft_isalnum
```
int ft_isalnum ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Checks whether *c* is either a decimal digit or an uppercase or lowercase letter. | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_isalpha
```
int ft_isalpha ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Checks if character is alphabetic | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_isascii
```
int	ft_isascii(int c);
```
|Description | Parameters | Return Value|
|---|---|---|
|Checks if character is an ASCII character | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_isdigit
```
int ft_isdigit ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Checks if character is decimal digit | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_isprint
```
int ft_isprint ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Checks if character is printable | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_memchr
```
void	*ft_memchr(const void *s, int c, size_t n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Locate character in block of memory | *s* - pointer to a block of memory; *c* - character searched in s; *n* - number of bytes |A pointer to the first occurrence of *c* in the block of memory pointed by *s*; Else - NULL-pointer|
#### ft_memcmp
```
int	ft_memcmp(const void *s1, const void *s2, size_t n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Compare two blocks of memory | *s1* - first block of memory; *s2* - secondl block of memory; *n* - number of bytes to compare|*<0* - if the first byte has a lower value than the second; *0* - if blocks are equal; *>0* if the first byte has a greater value than the second|
#### ft_memcpy
```
void	*ft_memcpy(void *dst, const void *src, size_t n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Copy block of memory| *dst* - where to copy; *src* - source to be copied; *n* - number of bytes to copy|dst|
#### ft_memmove
```
void	*ft_memmove(void *dst, const void *src, size_t n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Move block of memory; Does not check terminating NULL -> dst an src can overlap| *dst* - where to copy; *src* - source to be copied; *n* - number of bytes to copy|dst|
#### ft_memset
```
void	*ft_memset(void *b, int c, size_t len);
```
|Description | Parameters | Return Value|
|---|---|---|
|Fill block of memory| *b* - where to set *len* bytes to *c* value|b|
#### ft_strchr
```
char	*ft_strchr(const char *s, int c);
```
|Description | Parameters | Return Value|
|---|---|---|
|Locate first occurrence of character in string| *s* - pointer to a string where to search; *c* - character to be searched|A pointer to the first occurrence of *c* in *s*|
#### ft_strdup
```
char	*ft_strdup(const char *s1);
```
|Description | Parameters | Return Value|
|---|---|---|
|Duplicate string| *s1* - pointer to a string to be duplicated|A pointer to a duplicated string|
#### ft_strlcat
```
size_t	ft_strlcat(char *dst, const char *src, size_t size);
```
|Description | Parameters | Return Value|
|---|---|---|
|Concatenate two strings| *dst* - pointer to a destination string; *src* - pointer to a source string; *size* - number of characters to append|Length of the new string|
#### ft_strlcpy
```
size_t	ft_strlcpy(char *dst, const char *src, size_t dstsize);
```
|Description | Parameters | Return Value|
|---|---|---|
|Copies characters from one string to another| *dst* - pointer to a destination string; *src* - pointer to a source string; *dstsize* - number of characters to be copied|Length of the new string|
#### ft_strlen
```
size_t	ft_strlen(const char *str);
```
|Description | Parameters | Return Value|
|---|---|---|
|Get string length| *str* - pointer to a string|length of string|
#### ft_strncmp
```
int	ft_strncmp(const char *s1, const char *s2, size_t n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Compare characters of two strings| *s1* - pointer to a first string *s2* - pointer to a second string; *n* - number of bytes to compare|A*<0* - if the first character has a lower value than the second; *0* - if strings are equal; *>0* if the first character has a greater value than the second|
#### ft_strnstr
```
char	*ft_strnstr(const char *s1, const char	*s2, size_t	n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Locates substring| *s1* - pointer to a first string *s2* - pointer to a second string; *n* - number of bytes to search for|A pointer to the first character of the first occurrence of little is returned. NULL if the substring is not found. If *s2* is an empty string, *s1* is returned|
#### ft_strrchr
```
char	*ft_strrchr(const char *s, int c);
```
|Description | Parameters | Return Value|
|---|---|---|
|Locate last occurrence of character in string| *s* - pointer to a string where to seacrh; *c* - a character to search for|A pointer to last occurence *c* in *s*|
#### ft_tolower
```
int tolower ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Convert uppercase letter to lowercase | *c* - a character to be converted |The lowercase equivalent to c|
#### ft_toupper
```
int tolower ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Convert lowercase letter to uppercase | *c* - a character to be converted |The uppercase equivalent to c|
### Additional
#### ft_itoa
```
char *ft_itoa(int n);
```
|Description | Parameters | Return Value|
|---|---|---|
|Allocates and returns a string representing the integer received as an argument. |*n* - the integer to convert.|The string representing the integer. NULL if the allocation fails.|
#### ft_putchar_fd
```
void ft_putchar_fd(char c, int fd);
```
|Description | Parameters | Return Value|
|---|---|---|
|Outputs the character ’c’ to the given file descriptor |*c* - The character to output;*fd* - The file descriptor on which to write.|---|
#### ft_putendl_fd
```
void ft_putendl_fd(char *s, int fd);
```
|Description | Parameters | Return Value|
|---|---|---|
|Outputs the string ’s’ to the given file descriptor followed by a newline.|*s* -  The string to output; *fd* - The file descriptor on which to write|---|
#### ft_putnbr_fd
```
void ft_putnbr_fd(int n, int fd);
```
|Description | Parameters | Return Value|
|---|---|---|
|Outputs the integer ’n’ to the given file descriptor|*n* -  The integer to output. *fd* - The file descriptor on which to write.|---|
#### ft_putstr_fd
```
void ft_putstr_fd(char *s, int fd);
```
|Description | Parameters | Return Value|
|---|---|---|
|Outputs the string ’s’ to the given file descriptor.|*s* - The string to output. *fd* -The file descriptor on which to write|---|
#### ft_split
```
char **ft_split(char const *s, char c);
```
|Description | Parameters | Return Value|
|---|---|---|
|Allocates and returns an array of strings obtained by splitting ’s’ using the character ’c’ as a delimiter. The array must end with a NULL pointer|*s* - The string to be split; *c* -  The delimiter character|The array of new strings resulting from the split.NULL if the allocation fails|
#### ft_striteri
```
void ft_striteri(char *s, void (*f)(unsigned int, char*));
```
|Description | Parameters | Return Value|
|---|---|---|
|Applies the function ’f’ on each character of the string passed as argument, passing its index as first argument. Each character is passed by address to ’f’ to be modified if necessary.|*s* - The string on which to iterate; *f* - The function to apply to each character. |---|
#### ft_strjoin
```
char *ft_strjoin(char const *s1, char const *s2);
```
|Description | Parameters | Return Value|
|---|---|---|
|Allocates and returns a new string, which is the result of the concatenation of ’s1’ and ’s2’|*s1* - The prefix string; *s2* -  The suffix string.|The new string. NULL if the allocation fails.|
#### ft_strmapi
```
char *ft_strmapi(char const *s, char (*f)(unsigned int, char));
```
|Description | Parameters | Return Value|
|---|---|---|
|Applies the function ’f’ to each character of the string ’s’, and passing its index as first argument to create a new string resulting from successive applications of ’f’|*s* - The string on which to iterate; *f* -The function to apply to each character|The string created from the successive applications of ’f’. Returns NULL if the allocation fails|
#### ft_strtrim
```
char *ft_strtrim(char const *s1, char const *set);
```
|Description | Parameters | Return Value|
|---|---|---|
|Allocates and returns a copy of ’s1’ with the characters specified in ’set’ removed from the beginning and the end of the string|*s1* - The string to be trimmed; *set* - The reference set of characters to trim|The trimmed string. NULL if the allocation fails|
#### ft_substr
```
char *ft_substr(char const *s, unsigned int start, size_t len);
```
|Description | Parameters | Return Value|
|---|---|---|
|Allocates and returns a substring from the string ’s’. The substring begins at index ’start’ and is of maximum size ’len’|*s* - The string from which to create the substring; *start* - The start index of the substring in the
string ’s’; *len* - The maximum length of the substring|The substring.
NULL if the allocation fails|
### Bonus
#### ft_lstadd_back
```
void ft_lstadd_back(t_list **lst, t_list *new);
```
|Description | Parameters | Return Value|
|---|---|---|
|Adds the node ’new’ at the end of the list.|*lst* - The address of a pointer to the first link of a list; *new* - The address of a pointer to the node to be added to the list|---|
#### ft_lstadd_front
```
void ft_lstadd_front(t_list **lst, t_list *new);
```
|Description | Parameters | Return Value|
|---|---|---|
|Adds the node ’new’ at the beginning of the list.|*lst* - The address of a pointer to the first link of a list; *new* - The address of a pointer to the node to be added to the list|---|
#### ft_lstclear
```
void ft_lstclear(t_list **lst, void (*del)(void*));
```
|Description | Parameters | Return Value|
|---|---|---|
|Deletes and frees the given node and every successor of that node, using the function ’del’ and free. Finally, the pointer to the list must be set to NULL|*lst* - The address of a pointer to a node; *del* - The address of the function used to delete the content of the node|---|
#### ft_lstdelone
```
void ft_lstdelone(t_list *lst, void (*del)(void*));
```
|Description | Parameters | Return Value|
|---|---|---|
|Takes as a parameter a node and frees the memory of the node’s content using the function ’del’ given as a parameter and free the node. The memory of ’next’ must not be freed|*lst* - The node to free; *del* - The address of the function used to delete the content|---|
#### ft_lstiter
```
void ft_lstiter(t_list *lst, void (*f)(void *));
```
|Description | Parameters | Return Value|
|---|---|---|
|Iterates the list ’lst’ and applies the function ’f’ on the content of each node|*lst* - The address of a pointer to a node; *f* - The address of the function used to iterate on the list|---|
#### ft_lstlast
```
t_list *ft_lstlast(t_list *lst);
```
|Description | Parameters | Return Value|
|---|---|---|
|Returns the last node of the list|*lst* - The beginning of the list|Last node of the list|
#### ft_lstmap
```
t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));
```
|Description | Parameters | Return Value|
|---|---|---|
|Iterates the list ’lst’ and applies the function ’f’ on the content of each node. Creates a new list resulting of the successive applications of the function ’f’. The ’del’ function is used to delete the content of a node if needed|*lst* - The address of a pointer to a node; *f* - The address of the function used to iterate on the list; *del* - The address of the function used to delete the content of a node if needed|The new list. NULL if the allocation fails|
#### ft_lstnew
```
t_list *ft_lstnew(void *content);
```
|Description | Parameters | Return Value|
|---|---|---|
|Allocates and returns a new node. The member variable ’content’ is initialized with the value of the parameter ’content’. The variable ’next’ is initialized to NULL| *content* - The content to create the node with.| The new node|
#### ft_lstsize
```
int ft_lstsize(t_list *lst);
```
|Description | Parameters | Return Value|
|---|---|---|
|Counts the number of nodes in a list|*lst* - The beginning of the list|The length of the list|

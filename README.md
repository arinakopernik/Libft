![libft](https://user-images.githubusercontent.com/103765789/168682988-b193a664-22e7-4751-ad12-620adca7d073.JPG)

# Libft
Libft is the very first individual project at School21. It's goal is to recode a few functioins from C standart library and some extra functions. It's goal is to create a library that we'll be able to use in our future projects as we are not allowed to use standart libraries. Also. it helps us to understand the basic algorithms.
## Functions
| Mandatory | Additional | Bonus |
|---|---|---|
|[ft_atoi](#ft_atoi)|ft_itoa | ft_lstadd_back
|[ft_bzero](#ft_bzero) | ft_putchar_fd |ft_lstadd_front
|[ft_calloc](#ft_calloc) | ft_putendl_fd | ft_lstclear
|[ft_isalnum](#ft_isalnum) | ft_putnbr_fd | ft_lstdelone
|[ft_isalpha](#ft_isalpha) | ft_putstr_fd | ft_lstiter
|[ft_isascii](#ft_isascii) | ft_split | ft_lstlast
|[ft_isdigit](#ft_isdigit) | ft_striteri |ft_lstmap
|[ft_isprint](#ft_isprint) | ft_strjoin |ft_lstnew
|[ft_memchr](#ft_memchr) | ft_strmapi | ft_lstsize
|[ft_memcmp](#ft_memcmp) | ft_strtrim | 
|[ft_memcpy](#ft_memcpy) | ft_substr
|[ft_memmove](#ft_memmove) 
|[ft_memset](#ft_memset) 
|[ft_split](#ft_split)
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
int isalnum ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Checks whether *c* is either a decimal digit or an uppercase or lowercase letter. | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_isalpha
```
int isalpha ( int c );
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
|Checks if character is an ASCII charachter | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_isdigit
```
int isdigit ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Checks if character is decimal digit | *c* - a value to be checked |True - a value different from 0; False - 0|
#### ft_isprint
```
int isprint ( int c );
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
|Locate character in block of memory | *s* - pointer to a block of memory; *c* - charachter searched in s; *n* - number of bytes |A pointer to the first occurrence of *c* in the block of memory pointed by *s*; Else - NULL-pointer|
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
#### ft_split
```
char	**ft_split(char const *s, char c);
```
|Description | Parameters | Return Value|
|---|---|---|
|Returns an array of strings splitting *s* using the character *c* as a delimiter. | *s* - pointer to a string to be splitted; *c* - delimiter|An array of strings|
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
char	*ft_strrchr(const char *s, int c)
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
|Convert uppercase letter to lowercase | *c* - a charachter to be converted |The lowercase equivalent to c|
#### ft_toupper
```
int tolower ( int c );
```
|Description | Parameters | Return Value|
|---|---|---|
|Convert lowercase letter to uppercase | *c* - a charachter to be converted |The uppercase equivalent to c|

# String and Memory Manipulation Functions

This repository contains a collection of string and memory manipulation functions written in C. These functions can be used to perform various operations on strings and memory blocks. Below is a brief description of each function along with its signature.

## `u32 my_strlength(const void *str1)`

This function calculates and returns the length of the null-terminated string pointed to by `str1`.

## `void my_strcpy(void *str1, const void *str2)`

This function copies the contents of the null-terminated string pointed to by `str2` to the location pointed to by `str1`.

## `void my_strncpy(void *str1, const void *str2, u32 n)`

This function copies up to `n` characters from the null-terminated string pointed to by `str2` to the location pointed to by `str1`.

## `void my_strcat(void *str1, const void *str2)`

This function appends the contents of the null-terminated string pointed to by `str2` to the end of the null-terminated string pointed to by `str1`.

## `void my_strncat(void *str1, const void *str2, u32 n)`

This function appends up to `n` characters from the null-terminated string pointed to by `str2` to the end of the null-terminated string pointed to by `str1`.

## `s32 my_memcmp(const void *str1, const void *str2, u32 n)`

This function compares the first `n` bytes of the memory blocks pointed to by `str1` and `str2` and returns an integer less than, equal to, or greater than zero, depending on whether `str1` is less than, equal to, or greater than `str2`.

## `void *my_memchr(const void *str, s32 c, u32 size)`

This function searches for the first occurrence of the byte `c` within the first `size` bytes of the memory block pointed to by `str` and returns a pointer to the matching byte, or NULL if the byte is not found.

## `u8 *my_strchr(const u8 *str, s32 c)`

This function searches for the first occurrence of the character `c` in the null-terminated string `str` and returns a pointer to the matching character, or NULL if the character is not found.

## `u8 *my_strrchr(const u8 *str, s32 c)`

This function searches for the last occurrence of the character `c` in the null-terminated string `str` and returns a pointer to the matching character, or NULL if the character is not found.

## `u8 *my_strstr(const u8 *s1, const u8 *s2)`

This function searches for the first occurrence of the substring `s2` in the null-terminated string `s1` and returns a pointer to the beginning of the substring, or NULL if the substring is not found.

## `u64 my_strcspn(const u8 *str1, const u8 *str2)`

This function calculates the length of the initial segment of `str1` that consists of characters not in `str2` and returns the count of characters.

## `u64 my_strspn(const u8 *str1, const u8 *str2)`

This function calculates the length of the initial segment of `str1` that consists of characters in `str2` and returns the count of characters.

## `u8 *my_strpbrk(const u8 *str1, const u8 *str2)`

This function searches `str1` for any of the characters in `str2` and returns a pointer to the first occurrence of any of these characters, or NULL if none of them are found.
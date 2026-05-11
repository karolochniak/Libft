# Libft 📚

A custom implementation of the standard C library (`libc`) along with additional utility functions. This project serves as a foundational static library (`libft.a`) designed to be reused in future C programming projects.

---

## 🎯 About the Project

In many low-level C projects, standard library functions are often restricted. `Libft` solves this by providing reliable, custom-built alternatives for memory management, string manipulation, character checking, and linked list operations. 

By compiling this repository, you generate a `libft.a` archive that can be seamlessly linked into any C project.

---

## 🧩 Features & Function Categories

The library is divided into three main categories based on the functionality provided.

### 1. Standard `libc` Equivalents
Core functions that replicate the behavior of the standard C library:
*   **Character Checks & Manipulation:** `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`, `ft_toupper`, `ft_tolower`
*   **String Manipulation:** `ft_strlen`, `ft_strchr`, `ft_strrchr`, `ft_strncmp`, `ft_strnstr`, `ft_strlcpy`, `ft_strlcat`, `ft_strdup`
*   **Memory Management:** `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`, `ft_memchr`, `ft_memcmp`, `ft_calloc`
*   **Conversion:** `ft_atoi`

### 2. Additional Utility Functions
Functions designed to handle common string parsing and file descriptor outputs:
*   **String Creation & Parsing:** `ft_substr`, `ft_strjoin`, `ft_strtrim`, `ft_split`, `ft_itoa`
*   **Function Mapping:** `ft_strmapi`, `ft_striteri`
*   **File Descriptor Output:** `ft_putchar_fd`, `ft_putstr_fd`, `ft_putendl_fd`, `ft_putnbr_fd`

### 3. Linked List Operations (Bonus)
A complete suite of tools to manage singly linked lists via the `t_list` structure:
*   `ft_lstnew`, `ft_lstadd_front`, `ft_lstsize`, `ft_lstlast`, `ft_lstadd_back`
*   `ft_lstdelone`, `ft_lstclear`, `ft_lstiter`, `ft_lstmap`

---

## 🛠️ Compilation

The project includes a `Makefile` to easily compile the source files into the static library `libft.a`.

### Available `make` commands:

*   `make` or `make all` - Compiles the mandatory core functions.
*   `make bonus` - Compiles the library including the linked list functions.
*   `make clean` - Removes the compiled `.o` object files.
*   `make fclean` - Removes both the object files and the `libft.a` binary.
*   `make re` - Completely recompiles the library (runs `fclean` followed by `all`).

---

## 🚀 Usage

To use `Libft` in your own projects:

1. **Include the header** in your C files:
   ```c
   #include "libft.h"

# 42cursus - get_next_line

This project requires writing a function `get_next_line()` in C that reads a line from a file descriptor, one line at a time. The function should handle both file and standard input, returning a line that includes the terminating newline character unless the file ends without one. The project introduces the concept of static variables in C, helping you understand how to manage memory and control state across multiple function calls.

## Features

* The function `get_next_line(int fd)` should return a line from the file associated with the provided file descriptor.
* The function should return `NULL` when there's nothing mor to read or if an error occur.
* The function should read in chunks with a defined buffer size (`BUFFER_SIZE`), allowing multiple calls to read lines progressively.
* Memory management is crucial; no memory leaks should occur.
* The function should not use forbidden functions like `lseek()` or global variables.

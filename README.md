<h1 align="center">42_GET_NEXT_LINE_1337</h1>
<p align="center">
  <a href="https://github.com/haytham-hammioui/42_Get_next_line_1337">
    <img src="https://raw.githubusercontent.com/ayogun/42-project-badges/refs/heads/main/badges/get_next_linem.png" alt="42 Badge">
  </a>
</p>

# get_next_line

**get_next_line** is a versatile C function designed for efficient and dynamic line reading from file descriptors. This implementation is part of the 42 school curriculum and serves as a crucial component for handling file input in C programs. Master the art of reading lines, dynamically allocating memory, and enhancing your file processing capabilities with `get_next_line`.

## Getting Started

### Installation

1. **Clone the Repository**
   ```sh
   git clone https://github.com/haytham-hammioui/42_Get_next_line_1337.git GNL
   ```

2. Include the `get_next_line.h` or `get_next_line_bonus.h` files in your project.

### Usage

To use `get_next_line` in your C projects:

1. Compile your project with `get_next_line.c` and `get_next_line_bonus.c`:

    ```bash
    gcc -Wall -Wextra -Werror -D BUFFER_SIZE=your_buffer_size your_source_files.c get_next_line.c get_next_line_utils.c -o your_executable
    ```

    Replace `your_buffer_size` with the desired buffer size (e.g., 32, 64).

4. Use `get_next_line` in your code:

    ```c
    #include "get_next_line.h"

    int main(void) {
        int fd;
        char *line;

        // Open your file descriptor (fd) here
        fd = open("PATH_TO_FILE", O_RDWR);
        line = get_next_line(fd);

       printf("%s\n", line);
       free(line);

        // Close your file descriptor (fd) here
        close(fd);

        return 0;
    }
    ```

    Make sure to handle errors appropriately and free allocated memory when done.

## Contributing

Contributions to `get_next_line` are welcome! Whether you've found a bug, have a feature request, or want to contribute code:

1. Fork the repository.
2. Create a new branch for your changes.
3. Add your contributions.
4. Push your branch and open a pull request against the `get_next_line` repository.

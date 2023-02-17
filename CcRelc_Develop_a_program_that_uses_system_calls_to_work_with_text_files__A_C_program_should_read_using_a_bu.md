

# **Solution using System Calls to Work with Text Files**

Here, we will develop a C program which reads a file using a buffer larger than the readable files and writes the read file to a file with a different name. The file names to read and write from will be specified as command line arguments.

## Algorithm

The following algorithm outlines the steps for the program: 

1. Set the file name to read and write from as command line arguments.
2. Create a buffer larger than the size of the readable file.
3. Open the file to read from.
4. Read the file using the created buffer.
5. Create a new file and open it to write the read content.
6. Write the content of the file into the new file using the created buffer.
7. Close both the files.

## Code

The following code implements the above algorithm:

```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[])
{
    // Set file names to read and write from as command line arguments
    char *inputFileName = argv[1];
    char *outputFileName = argv[2];
 
    // Create a buffer larger than the size of the readable file
    char buffer[20];
 
    // Open the file to read from
    FILE *inputFile = fopen(inputFileName, "r");
 
    // Read the file using the created buffer
    size_t bytesRead = fread(buffer, 1, sizeof(buffer), inputFile);
 
    // Create a new file and open it to write the read content
    FILE *outputFile = fopen(outputFileName, "w");
 
    // Write the content of the file into the new file using the created buffer
    size_t bytesWritten = fwrite(buffer, 1, bytesRead, outputFile);
 
    // Close both the files
    fclose(inputFile);
    fclose(outputFile);
 
    return 0;
}
```

## Explanation

The program begins by setting the file names to read and write from as command line arguments. After that, a buffer is created which is larger than the size of the readable file. We then open the file to read from and read the file using the created buffer. We then create a new file and open it to write the read content into. The content of the file is then written into the new file using the created buffer. Finally, both the files are closed.
# Read: Class 19

1. **How can you use regular expressions in Python to search for specific patterns in a string, and what is the primary module to work with them?**

To use regular expressions in Python, you can use the re module, which provides support for regular expressions. The re module allows you to search, match, and manipulate strings based on specific patterns.

2. **What is the purpose of the shutil module in Python, and provide an example of a common use case for file or directory management with this module?**

The shutil module in Python provides a higher-level interface for file operations, including file and directory management. It simplifies common file-related tasks like copying, moving, and removing files and directories.

Example:

`import shutil`

`source_file = 'source.txt'`
`destination = 'destination_folder/'`

`shutil.copy(source_file, destination)`

3. **Compare and contrast the os and shutil modules. When would you choose to use one over the other?**

os module: It provides a way of using operating system-dependent functionality like reading or writing to the file system, creating directories, etc. It's more focused on lower-level, platform-specific operations.

shutil module: It builds on top of the os module and provides higher-level file operations that are more user-friendly and platform-independent. It is especially useful for common file and directory management tasks.

When to choose one over the other:

Use os when you need low-level operations and want more control over the details.

Use shutil when you want a higher-level interface for common file and directory management tasks, and you want to write more concise and readable code.

Example: If you just need to copy or move a file, shutil is often a better choice for simplicity and readability. If you need to perform more complex operations or interact directly with the operating system, then os might be more appropriate.

## `Things I want to know more about`

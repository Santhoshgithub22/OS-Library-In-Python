# OS-Library-In-Python

The os module in Python provides a way to interact with the operating system, allowing you to perform various tasks such as file and directory operations, environment variables manipulation, and executing system commands. Here's a brief overview of some commonly used functionalities provided by the os module:

Working with Files and Directories:

* os.getcwd(): Get the current working directory.
* os.chdir(path): Change the current working directory to the specified path.
* os.listdir(path='.'): List files and directories in the specified directory.
* os.mkdir(path): Create a new directory.
* os.makedirs(path): Create directories recursively.
* os.remove(path): Remove a file.
* os.rmdir(path): Remove an empty directory.
* os.removedirs(path): Remove directories recursively.
* os.rename(src, dst): Rename a file or directory.
* os.path.exists(path): Check if a path exists.

Environment Variables:

* os.environ: A dictionary containing the environment variables.
* os.getenv(var_name, default=None): Get the value of the specified environment variable.
* os.putenv(var_name, value): Set the value of the specified environment variable.
* os.unsetenv(var_name): Unset (delete) the specified environment variable.

Miscellaneous:

* os.system(command): Execute the command in the system shell.
* os.path.join(path1, path2, ...): Join one or more path components intelligently.
* os.path.abspath(path): Return the absolute version of a path.
* os.path.basename(path): Return the base name of a path.
* os.path.dirname(path): Return the directory name of a path.
* os.path.isfile(path): Check if a path is a regular file.
* os.path.isdir(path): Check if a path is a directory.

Here's a simple example demonstrating the use of os module functions to work with files and directories:

Here are basic examples for each of the functionalities you listed:

```
import os
```

#### Get current working directory
```
cwd = os.getcwd()
print("Current working directory:", cwd)
```

#### List files and directories
```
files = os.listdir(cwd)
print("Files and directories in current directory:", files)
```

#### Create a new directory
```
new_dir = os.path.join(cwd, 'new_directory')
os.mkdir(new_dir)
```

#### Check if a path exists
```
path = os.path.join(cwd, 'file.txt')
if os.path.exists(path):
    print("Path exists:", path)
else:
    print("Path does not exist:", path)
```
```
import os
```

# Working with Files and Directories

#### Get the current working directory
```
cwd = os.getcwd()
print("Current working directory:", cwd)
```

#### Change the current working directory to the specified path
```
os.chdir('/path/to/new/directory')
print("New working directory:", os.getcwd())
```

#### List files and directories in the specified directory
```
files = os.listdir()
print("Files and directories:", files)
```

#### Create a new directory
```
os.mkdir('new_directory')
```

#### Create directories recursively
```
os.makedirs('parent_dir/sub_dir')
```

#### Remove a file
```
os.remove('file.txt')
```

#### Remove an empty directory
```
os.rmdir('empty_directory')
```

#### Remove directories recursively
```
os.removedirs('parent_dir/sub_dir')
```

#### Rename a file or directory
```
os.rename('old_name.txt', 'new_name.txt')
```

#### Check if a path exists
```
if os.path.exists('file.txt'):
    print("Path exists")
else:
    print("Path does not exist")
```

# Environment Variables

#### Get the value of the specified environment variable
```
home_dir = os.getenv('HOME')
print("Home directory:", home_dir)
```

#### Set the value of the specified environment variable
```
os.putenv('MY_VAR', 'value')
```

#### Unset (delete) the specified environment variable
```
os.unsetenv('MY_VAR')
```

# Miscellaneous

#### Execute the command in the system shell
```
os.system('ls -l')
```

#### Join one or more path components intelligently
```
path = os.path.join('/path/to', 'directory', 'file.txt')
print("Joined path:", path)
```

#### Return the absolute version of a path
```
abs_path = os.path.abspath('file.txt')
print("Absolute path:", abs_path)
```

#### Return the base name of a path
```
basename = os.path.basename('/path/to/file.txt')
print("Base name:", basename)
```

#### Return the directory name of a path
```
dirname = os.path.dirname('/path/to/file.txt')
print("Directory name:", dirname)
```

#### Check if a path is a regular file
```
print("Is file?", os.path.isfile('/path/to/file.txt'))
```

#### Check if a path is a directory
```
print("Is directory?", os.path.isdir('/path/to/directory'))
```

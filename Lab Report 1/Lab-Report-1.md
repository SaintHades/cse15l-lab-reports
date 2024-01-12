# Lab Report 1


## cd

### 1. with no arguments
```
[user@sahara ~]$ cd
[user@sahara ~]$
```
  * working directory: /home
  * When using `cd` with no argument, it will back to the root directory no matter what the working directory at. In this case, the working directory is the root directory, so nothing changed.
  * not error

### 2. with *directory* as arguments
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$
```
  * working directory: /home, change to /home/lecture1 after the command run
  * When using `cd` with *directory* as arguments, the working directory will change to the specific directory which the path we given as the argument.
  * not error

### 3. with *file* as arguments
```
[user@sahara ~/lecture1]$ cd Hello.java
bash: cd: Hello.java: Not a directory
```
  * working directory: /home/lecture1
  * When using `cd` with *file* as arguments, it showing an error. The reason is that `cd` is only able to take an existing or reasonable path as an argument and switch to that directory as the working directory.
  * error, since a *file* is passed in as an argument, which is not a path, and `cd` only can take the path as an argument. 


## ls

### 1. with no arguments
```
[user@sahara ~/lecture1]$ ls 
Hello.class  Hello.java  messages  README
```
  * working directory: /home/lecture1
  * When using `ls` with no arguments, it will list all files or folders within the working directory.
  * not error

### 2. with *directory* as arguments
```
[user@sahara ~/lecture1]$ ls messages
en-us.txt  es-mx.txt  th.txt  zh-cn.txt
```
  * working directory: /home/lecture1
  * When using `ls` with *directory* as arguments, it will list all files or folders within the directory that we give as the parameter.
  * not error

### 3. with *file* as arguments
```
[user@sahara ~/lecture1]$ ls Hello.java
Hello.java
```
  * working directory: /home/lecture1
  * When using `ls` with *file* as arguments, it shows the relative path of the file. In this case, Hello.java is in the current working directory, in which the output is just the file name.
  * not error

## cat

### 1. with no arguments
[Image] cat1.png
```
[user@sahara ~/lecture1]$ cat
test
test
test1
test1
test2
test2
```
  * working directory: /home/lecture1
  * When using `cat` with no arguments, it turns to a working space that will just repeat showing what we type in the working space, and `ctrl + c` will that us to exit the working space.
  * not error

### 2. with *directory* as arguments
```
[user@sahara ~/lecture1]$ cat messages
cat: messages: Is a directory
```
  * working directory: /home/lecture1
  * When using `cat` with *directory* as arguments, it causes an error, since `cat` is only able to take *file* as arguments.
  * error, since a 

### 3. with *file* as arguments
```
[user@sahara ~/lecture1]$ cat Hello.java
import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }
}
```
  * working directory: /home/lecture1
  * TODO
  * error, TODO

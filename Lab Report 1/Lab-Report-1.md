# Lab Report 1


## cd

### 1. with no arguments
```
[user@sahara ~]$ cd
[user@sahara ~]$
```
  * working directory: /home
  * TODO
  * not error

### 2. with *directory* as arguments
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$
```
  * working directory: /home
  * TODO
  * not error

### 3. with *file* as arguments
```
[user@sahara ~/lecture1]$ cd Hello.java
bash: cd: Hello.java: Not a directory
```
  * working directory: /home/lecture1
  * TODO
  * error


## ls

### 1. with no arguments
```
[user@sahara ~/lecture1]$ ls 
Hello.class  Hello.java  messages  README
```
  * working directory: /home/lecture1
  * 
  * not error

### 2. with *directory* as arguments
```
[user@sahara ~/lecture1]$ ls messages
en-us.txt  es-mx.txt  th.txt  zh-cn.txt
```
  * working directory: /home/lecture1
  * TODO
  * not error

### 3. with *file* as arguments
```
[user@sahara ~/lecture1]$ ls Hello.java
Hello.java
```
  * working directory: /home/lecture1
  * TODO
  * not error

## cat

### 1. with no arguments
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
  * TODO
  * not error

### 2. with *directory* as arguments
```
[user@sahara ~/lecture1]$ cat messages
cat: messages: Is a directory
```
  * working directory: /home/lecture1
  * TODO
  * error, TODO

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

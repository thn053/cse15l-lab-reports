# CSE15L LAB1
## 1) cd command
```
{
oceenguyen@Ocees-MacBook-Air lecture1 % cd
oceenguyen@Ocees-MacBook-Air ~ % pwd
/Users/oceenguyen
oceenguyen@Ocees-MacBook-Air ~ % cd lecture1
oceenguyen@Ocees-MacBook-Air lecture1 % pwd
/Users/oceenguyen/lecture1
oceenguyen@Ocees-MacBook-Air lecture1 % cd non_existent_folder
cd: no such file or directory: non_existent_folder
oceenguyen@Ocees-MacBook-Air lecture1 % pwd
/Users/oceenguyen/lecture1
}
```
## Example 1: Using cd with No Arguments "cd"
-Current Directory: The current directory is the home directory /Users/oceenguyen.
-Output Explanation: When you use cd without any arguments, it takes you to your home directory.
## Example 2: Using cd with a Directory Path "cd lecture1"
-Current Directory: Now we are in /Users/oceenguyen/lecture1.
-Output Explanation: This command changes the current directory to the lecture1 folder within the home directory.
## Example 3: Using cd with an Invalid Path "cd non_existent_folder"
-Current Directory: We are still in /Users/oceenguyen/lecture1.
-Output Explanation: An error occurs because non_existent_folder does not exist.
## 2) ls command
```
{
oceenguyen@Ocees-MacBook-Air lecture1 % ls
Hello.class	Hello.java	README		lecture1	messages
oceenguyen@Ocees-MacBook-Air lecture1 % pwd
/Users/oceenguyen/lecture1
oceenguyen@Ocees-MacBook-Air lecture1 % ls lecture1
Hello.java	README		messages
oceenguyen@Ocees-MacBook-Air lecture1 % pwd
/Users/oceenguyen/lecture1
oceenguyen@Ocees-MacBook-Air lecture1 % ls Hello.class
Hello.class
oceenguyen@Ocees-MacBook-Air lecture1 % pwd
/Users/oceenguyen/lecture1
}
```
## Example 4: Using ls with No Arguments "ls"
-Current Directory: We are still in /Users/oceenguyen/lecture1.
-Output Explanation: Lists files and folders in the current directory.
## Example 5: Using ls with a Directory Path "ls lecture1"
-Current Directory: We are still in /Users/oceenguyen/lecture1.
-Output Explanation: Lists files and folders in the lecture1 directory.
## Example 6: Using ls with an Invalid Path "ls Hello.class "
-Current Directory: We are still in /Users/oceenguyen/lecture1.
-Output Explanation: Lists files and folders in the Hello.class directory.
## 3) cat command
```
{
oceenguyen@Ocees-MacBook-Air lecture1 % cat Hello.java
import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }
}%                                                                              oceenguyen@Ocees-MacBook-Air lecture1 % cat lecture1
cat: lecture1: Is a directory
oceenguyen@Ocees-MacBook-Air lecture1 % cat Hello.java Hello.class
import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }
}????A2

java/lang/Object<init>()java/lang/String




java/nio/file/Pathof;(Ljava/lang/String;[Ljava/lang/String;)Ljava/nio/file/Path;
                                                                               !java/nio/charset/StandardCharsetsUTF_8Ljava/nio/charset/Charset;

java/nio/file/Files
readStringB(Ljava/nio/file/Path;Ljava/nio/charset/Charset;)Ljava/lang/String;	
                                                                                java/lang/SystemoutLjava/io/PrintStream;
"#$
   %&java/io/PrintStreamprintln(Ljava/lang/String;)V(HelloCodeLineNumberTablemain([Ljava/lang/String;)V
Exceptions/java/io/IOException
SourceFile
Hello.java!')*??*	+,)9*2??	??L?!?*
-.01%
}
```
## Example 7: Using cat with a File "cat Hello.java"
-Current Directory: We are still in /Users/oceenguyen/lecture1.
-Output Explanation: Displays the content of Hello.java.
## Example 8: Example 8: Using cat with an Invalid File "cat lecture1"
-Current Directory: We are still in /Users/oceenguyen/lecture1.
-Output Explanation: An error occurs because lecture1: Is a directory not a file.
## Using cat with Multiple Files "cat Hello.java Hello.class"
-Current Directory: We are still in /Users/oceenguyen/lecture1.
-Output Explaination: Concatenates and displays the content of Hello.java followed by Hello.class.







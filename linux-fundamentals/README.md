# Package management 

 > ### apt & apt-get : Current and classic command respectively
 > - **`apt install` :** Install a particular package 
 > - **`apt remove` :** Delete a particular package
 > - **`apt list` :** List of packages available for installation
 > - **`apt autoremove` :** Remove all packages that are not being used by others
 > - **`apt update` :** Synchronizes the database of locally available packages with the central storage. 
 
# File system 


# File and directory management 

* > **mkdir** 
* > **mv**
* > **touch**
* > **rm**
# File editing and viewing 

  > * > **cat** 
  > * > **more**
  > * > **less** 
  > * > **head**  
  > * > **tail** 

# Redirections 

> Redirects in Linux are best understood when you know the concept of **standard input and output streams**.In Unix and Linux, each process has three predefined standard streams : 
> - > **stdin :** Refers to the data stream that a program receives as input.By default, this is the keyboard.
> - > **stdout :** This is the stream of data that a program sends as output.By default, this is the terminal screen.
> - > **stderr :** This is the data stream for error messages.By default, it is also the terminal screen.
> ## Standard Output Redirection (stdout)

> * > **comando > archivo.txt :**
>   > - `cat archivo1.txt > archivo2.txt`
>   > - `cat archivo1.txt archivo2.txt > archivo3.txt`
>   > - `cat archivo1.txt archivo2.txt > archivo3.txt`
>   > - `echo "texto texto texto" > archivo1.txt`
> * > **comando >> archivo.txt :** 
>   > - `echo "texto texto texto" >> archivo1.txt`
>   > - `echo archivo1.txt >> archivo2.txt`
> ## Standard Input Redirection (stdin)
> - > **comando < archivo.txt :** 
        >   - Hola Hola 
> ## Standard Error Redirect (stderr)
> - > **comando 2> errores.txt :** 
> - > **comando 2>> errores.txt :** 
> - > **comando &> salida_y_errores.txt :** 
> - > **comando &>> salida_y_errores.txt :** 

# Text search 

# Search for files and directories 

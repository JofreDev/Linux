# Package management 

 > ### apt & apt-get : Current and classic command respectively
 > - **`apt install` :** Install a particular package 
 > - **`apt remove` :** Delete a particular package
 > - **`apt list` :** List of packages available for installation
 > - **`apt autoremove` :** Remove all packages that are not being used by others
 > - **`apt update` :** Synchronizes the database of locally available packages with the central storage. 
 
# File system 


# File and directory management 

* > **mkdir :** Create a new folder 
* > **mv :** It is versatile and is used for both moving and renaming files and directories
* > **touch :** Create files 
* > **rm :** Delete files and folders
# File editing and viewing 
  > * > **File viewing :**
  >   > - **cat :** Displays and concatenates files
  >   >   - `cat text1.txt`
  >   >   - `cat -n archivo.txt`
  >   > - **more :** Displays files in paginated form
  >   >   - `more archivo.txt`
  >   > - **less :** Displays files in paginated form with advanced navigation
  >   >   - `less archivo.txt`
  >   >   ```markdown
  >   >   
  >   >   Common Functions:
  >   >   
  >   >     Navigation:
  >   >       Press Enter to advance one line.
  >   >       Press Space to go forward one page.
  >   >       Press b to go back one page.
  >   >       Press q to exit.
  >   >     Search:
  >   >       Press / followed by a search term to search forward.
  >   >       Press ? followed by a search term to search backward.
  >   >   ```
  >   > - **head :** Displays the first lines of a file
  >   >   - `head archivo.txt`
  >   >   - `head -n 20 archivo.txt`
  >   >   ```sh
  >   >    jeoliver@pop-os:~$ head -n 2 frutas.txt 
  >   >    manzana
  >   >    pera
  >   >    jeoliver@pop-os:~$ 
  >   >   ```
  >   > - **tail :** Displays the last lines of a file, with real-time tracking capability
  >   >    - `tail archivo.txt`
  >   >    - `tail -n 20 archivo.txt`
  >   >    - `tail -f archivo.log` 
  >   >   ```sh
  >   >   jeoliver@pop-os:~$ tail -n 2 frutas.txt 
  >   >   naranja
  >   >   plátano
  >   >   jeoliver@pop-os:~$ tail -f frutas.txt 
  >   >   manzana
  >   >   pera
  >   >   naranja
  >   >   plátano
  >   >   
  >   >   ```
  > * > **file creation and editing :**
  >   > - **nano :** It is a simple and fast text editor, ideal for quick editing of files from the terminal.


# Redirections 

> Redirects in Linux are best understood when you know the concept of **standard input and output streams**.In Unix and Linux, each process has three predefined standard streams : 
> - > **stdin :** Refers to the data stream that a program receives as input.By default, this is the keyboard.
> - > **stdout :** This is the stream of data that a program sends as output.By default, this is the terminal screen.
> - > **stderr :** This is the data stream for error messages.By default, it is also the terminal screen.
> ## Standard Output Redirection (stdout)

> * > **comando > archivo.txt :**
>   > - `cat archivo1.txt > archivo2.txt`
>   > - `cat archivo1.txt archivo2.txt > archivo3.txt`
>   > - `echo "texto texto texto" > archivo1.txt`
> * > **comando >> archivo.txt :** 
>   > - `echo "texto texto texto" >> archivo1.txt`
>   > - `echo archivo1.txt >> archivo2.txt`
## Standard Input Redirection (stdin)
> * **comando < archivo.txt :**
>   - `sort < file__alphabetically_disordered.txt`
>   ```sh
>   jeoliver@pop-os:~$ cat frutas.txt
>   manzana
>   pera
>   naranja
>   plátano
>   jeoliver@pop-os:~$ sort < frutas.txt
>   manzana
>   naranja
>   pera
>   plátano
>   jeoliver@pop-os:~$
>   ```

> * **comando < archivo.txt > archivo_out.txt:**
>   - `sort < file__alphabetically_disordered.txt > file__alphabetically_ordered. `
>   ```sh
>   jeoliver@pop-os:~$ cat frutas.txt 
>   manzana
>   pera
>   naranja
>   plátano
>   jeoliver@pop-os:~$ sort < frutas.txt > frutas_organizadadas.txt
>   jeoliver@pop-os:~$ cat frutas_organizadadas.txt 
>   manzana
>   naranja
>   pera
>   plátano
>   ```


> ## Standard Error Redirect (stderr)
> * > **comando 2> errores.txt :**
>   > - `ls archivo_dose_not_exist.txt 2> errores.txt`
> * > **comando 2>> errores.txt :**
>   > - `ls -al archivo_dose_not_exist.txt 2>> errores.txt`
> * > **comando &> salida_y_errores.txt :**
>   > - `ls -la archivo_no.txt &> errs.txt` 
> * > **comando &>> salida_y_errores.txt :**
>   > - `ls -la archivo_no.txt &>> errs.txt` 
> * > **comando > salida_y_errores.txt 2>&1 :**
>   > - `ls -la archivo_no.txt > errs.txt 2>&1`
> * > **comando >> salida_y_errores.txt 2>&1 :**
> * > - `ls -la archivo_no.txt >> errs.txt 2>&1` 

# Text search 

# Search for files and directories 

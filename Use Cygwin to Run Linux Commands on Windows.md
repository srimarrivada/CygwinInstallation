# Install Cygwin to Run Linux Commands on Windows

**Cygwin** is a project developed using a collection of open source tools that provide Linux OS look and feel like functionality on Windows. 

Follow these steps to install Cygwin in Windows and use it. You can also go through [this](https://github.com/srimarrivada/CygwinInstallation/blob/main/Use%20Cygwin%20to%20Run%20Linux%20Commands%20on%20Windows.pdf) document with more detailed steps along with screenshots.

## **Cygwin Installation:**
Download Cygwin setup tool from the [official site](https://www.cygwin.com/) which provides us `setup-x86-64.exe` file to run.

After downloading `.exe` file, double-click on it to launch **Cygwin Setup** window and hit Next.

On **Cygwin Setup** window:
1. Choose the installation type: “Install from Internet” and hit Next.

2. Select the root installation directory where Cygwin needs to be installed (default install path is **C:/cygwin64** in Windows 64-bit OS) and choose if this installation is for you or for all users accessing the machine and click on Next.

3. Then, select a local directory where Cygwin needs to store installation files when it downloads. It shows the default location of where `.exe` file is launched. Change it if you wish to and press Next.
  
4. Next, select the option of how Cygwin needs to connect to Internet. You can leave default selection and press Next.
 
5. Then, choose a download site from the available list or mention a different download URL to add to this list and hit Next
   
6. Now, it starts downloading Cygwin from the chosen download URL.
  
7. Next, select Linux packages that you would want Cygwin to install and press Next
   
8. Review and confirm changes by pressing Next. It takes time to get selected packages downloaded.
   
9. Installation is completed and we are ready to use Cygwin now. Click on Finish to close the setup window. 

## **Cygwin Terminal Usage:**
To run Linux commands on the Cygwin terminal, start typing “Cygwin” in the Windows search bar and open Cygwin64 Terminal application. 
The first usage of Cygwin terminal may give the following messages just as an FYI.

```
Copying skeleton files.
These files are for the users to personalise their cygwin experience.
They will never be overwritten nor automatically updated.
'./.bashrc' -> '/home/hp//.bashrc'
'./.bash_profile' -> '/home/hp//.bash_profile'
'./.inputrc' -> '/home/hp//.inputrc'
'./.profile' -> '/home/hp//.profile'
 ```

Hurray!!, you can now play with Linux commands on Windows without Linux operating system.

**Example Basic Linux Commands:**<br>
Simply type a command on the terminal and press Enter to see results. <br>

1. Get present working directory <br>
   `pwd`

2. List all directories and files in the present working directory <br>
   `ls`

3. Navigate to specific directory <br>
   `cd <dirname>`

## Run Linux Commands on Windows Terminal:
Apart from Cygwin Terminal, we can also run Linux commands on Command Prompt itself. To do that, we need to add Cygwin path to Windows PATH environment variable. 

1. In the Windows search bar, start typing “environment variables” and select the first match.
   
2. On the “System Properties” window, click on “Environment Variables” button on the bottom right side.

3. Select **Path** variable under “System Variables” tab and press Edit.

4. Press New, add the path of `cygwin\bin` installation directory and Press OK.

5. After Path variable is updated, press OK on “Environment Variables” window to apply changes.

6. Open new Command Prompt shell and it now works like Linux terminal which accepts Linux commands.

\
***_Note:_*** <br>
When you try to execute non-basic Linux commands in Cygwin, you may get error “command not found”. 

For  example, run `nano` command: <br>
`nano <dirname> `

This error araise because the installed packages of Cygwin don’t support these commands. To use these commands, you have to start **Cygwin setup** by running `setup-x86-64.exe` file, keep pressing Next until you reach “select packages” where you have to select packages containing the functionality of this command.\

There you go! Now, you are free to execute Linux commands either on Windows Command Prompt or on Cygwin Terminal.

As a next step, you can refer [Linux Commands Cheat sheet](https://github.com/srimarrivada/LinuxCommands/blob/main/Linux%20Commands%20Cheat%20Sheet.docx) and start practicing.

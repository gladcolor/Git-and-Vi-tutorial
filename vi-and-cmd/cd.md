# Introduction  
`cd` is a command to do the changing directory in Linux command line interface. 
Before we do `cd`, let's look few simple concepts related to `cd`.    
For example, when we open the terminal or command line interface, we are on a default directory which is assained by system.  
This default directory is usually represented by special character **~**. For example, you can the blue **~** followed with green characters indicate the current place you are:  
![one](/image/vi/Screenshot from 2019-10-05 22-52-02.png)  
So, it means you are currently on a place what system calls it as **~**.
We start from the place shown on above picture and we first use command `pwd` to check the full directory path of where you current are:  
[]  
Ok, the **~** represents the directory **/home/ubuntu** and this is the place we currently stay.  
Now, we want to go to another directory. For instance, a directory under current directory. We can use `ls` to list every file and directory at current place:  
[]  
Say we want to go to directory **web**. Now it is time to offically introduce `cd`.  
# cd  
In Windows, you can just click mouse over a folder on screen. The command `cd` performs the same function as this mouse click in Windows.  
Type the `cd` at first and we follow with the directory we want to go. In this case, it is **web** directorty:  
[]  
Press enter, now you can see the blue character which shows the current your place append a **web** to the **~**. It means you successfully change the place to **web**.  
# Extra  
If you just type `cd` without anything, it directs you back to the default place **~**.  
If you just type `cd` with **..**, it leads you back to directory beofre the current place.  

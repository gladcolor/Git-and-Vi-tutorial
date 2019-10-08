# using the tab key to complete file path  
`Tab` key on your keyboard is really good tool to help you to do **auto-completion** of file names or directory names.  
For example, let's us open terminal use `ls` to check current files.  
![](/image/using_the_tab_key_to_complete_file_path/using_the_tab_key_to_complete_file_path_1.png)  
Say we want to use `vi` to open a file named **this_is_a_file_we_want_to_get_for_this_tutorial.txt**. But, no! It is to long for us to type its name, so we can use `Tab` key to do the auto-complete for its whole file name. Let's try to type **this** at first.  
![](/image/using_the_tab_key_to_complete_file_path/using_the_tab_key_to_complete_file_path_2.png)  
And then press `Tab` key  
![](/image/using_the_tab_key_to_complete_file_path/using_the_tab_key_to_complete_file_path_3.png)  
Whoo! We get it. Now we can just press enter to execute command, it saves us a lot time on file name typing.  
# Extra  
But, what if I want to have auto-completion based on a typed text whihc could also be a part of other non-target files?  
Say we still want to get file **this_is_a_file_we_want_to_get_for_this_tutorial.txt**, but now we just type a single **t** there and do the auto-completion. When we press the tab key at first time, it won't show anything. WHY? Becasue we have another file named **test.txt** under current directory. The system cannot distinguish whihc one you want to pick. However, if you press `Tab` key agin and every time after the second time, you will see the terminal will give you a list to show what are possible files you want to pick.  
![](/image/using_the_tab_key_to_complete_file_path/using_the_tab_key_to_complete_file_path_4.png)  
Now, you can try to type more text in order to get a distinct text which is easy for system to get the file name from your auto-completion.

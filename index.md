Hey y'all. Today we're gonna be doing some cool hackermans stuff.


A) Making your own Webserver

B) Remotely Connecting

C) Trying Some Commands


# PART A| Evading tips by making your own Server
![Image](https://www.springwise.com/wp-content/uploads/2018/03/Bear_Robotics_restaurant_Springwise.jpg)
![Image](https://media.minecraftstation.com/2020/08/Screen-Shot-2020-08-31-at-5.27.55-AM-1024x634.png)
(Disclaimer: may not be an accurate representation of what your Server will look like)


To install on vscode, click on this here link: [Link](https://code.visualstudio.com/download)

You should land on a page that looks like this:
![Image](vscode1.png) 

Select either Mac or Windows because if you're putting up with Linux, you don't need my help :)

Go ahead and run the installer.exe that spawned into your downloads folder. Just speedrun through the installer and make sure to skip all the parts that ask if you'd like to install a free trial of microsoft office /j. Anyways you'll know you've done it correctly after you land at an application window that looks like this:

<img width="960" alt="image" src="https://user-images.githubusercontent.com/130004918/231018113-c5140c12-e47e-4d32-83f3-1ddab238b385.png">
Congrats, you now have successfully installed vscode. And you have my blessing to move onto the next part



# PART B| ssh Time

If you have a Windows machine install gitbash here: [Link](https://gitforwindows.org/).
If you have a Mac, you're in the clear and don't need gitbash. The ssh should run directly in your terminal.
If you have a Linux machine, I can't help you :)

After all that jazz follow this guide: [Link](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit)

The guide should give you a username and password that you can enter into your terminal.

To remotely connect, open your terminal in VScode. [Note: for me, I couldn't connect because for some reason my previous VScode installation broke the ssh command, but switching to raw command prompt made it run. YMMV]


Copy and paste the following command into your terminal`ssh cs15lsp23**@ieng6.ucsd.edu`. Be sure to replace the ** with the letters that you got from following the google guide. On the next line it will ask for your password. If you type in or paste in something and you don't see anything that's normal. That's cyBeRseCuRiTY.
Hit enter after entering your password you should get some info that makes you look like a pro hacker like this:

<img width="497" alt="image" src="https://user-images.githubusercontent.com/130004918/231022374-a0f739eb-a586-4b84-8805-5fc8cece83e1.png">


# Part C| Hacking into the mainframe

Here we have some commands from Professor Pollitz:

`ls` - stands for "list" and will list files and directories in the current working directory

`ls -a` - a variation on the original list/`ls` command. Displays everything in the original `ls` command in addition to hidden files and directories

`ls -lat` - a variation on the original list/`ls` command. Displays everything in original `ls` command in a longer format with extra details such as permissions, details, time, size, and includes the hidden files from ls -a

(Notice how the same colored file names from `ls -a` can also be seen when entering `ls -lat`)

`cat /home/linux/ieng6/cs15lsp23/public/hello.txt` - stands for "concatenate" and prints the contents of a file. The `/home/linux/ieng6/cs15lsp23/public/hello.txt` part of the command is directory of the file that we are trying to concatenate.

These are just the ones that I used. There's a longer list in the original lab guidelines. Here's the final result.

<img width="848" alt="image" src="https://user-images.githubusercontent.com/130004918/231023185-1b6019d1-26e2-49c1-ab64-1947010996aa.png">

aaaaaaand that's it! You are done.

![image](https://user-images.githubusercontent.com/130004918/231045848-76984c65-7b64-4374-a309-b9e45da75f02.png)
r

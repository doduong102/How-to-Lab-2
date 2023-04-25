Hey y'all. Today we're going to be learning how to start your own "minecraft" server and bugspray your very own error-ridden java files


A) Making your own Webserver

B) Debugging

C) Takeaways from an amateur's perspective


# PART A| Evading tips by making your own Server
![Image](https://www.springwise.com/wp-content/uploads/2018/03/Bear_Robotics_restaurant_Springwise.jpg)
![Image](https://media.minecraftstation.com/2020/08/Screen-Shot-2020-08-31-at-5.27.55-AM-1024x634.png)
(Disclaimer: may not be an accurate representation of what your Server will look like)

In week 2 we created a NumberServer. After modifying the Handler class we can make it accept strings and perform somewhat similar functions. Another key modification is renaming the NumberServer class containing main to StringServer. Here's the changed code:
<img width="593" alt="image" src="https://user-images.githubusercontent.com/130004918/234173108-4e053fea-8326-4a6c-8ac0-a4ad838889be.png">

Which methods in your code are called?
What are the relevant arguments to those methods, and the values of any relevant fields of the class?
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

After compiling and running with the following commands:
```
⤇ javac Server.java StringServer.java 
⤇ java StringServer 3010
//We should get//
Server Started! Visit http://localhost:3010
```
Following the link it spat out...
We should land here
![image](https://user-images.githubusercontent.com/130004918/234174871-9df2d891-3158-41b3-92d1-2e1af833e328.png)
Now in the url we can test our /add-message implementation
Copying this 'http://localhost:3010/add-message?s=Hello' into the url should yield:
![image](https://user-images.githubusercontent.com/130004918/234175432-473cee12-3dfe-4434-a447-05d4f5470146.png)
Once more with 'http://localhost:3010/add-message?s=Hey, Hi, Hello' should yield:
![image](https://user-images.githubusercontent.com/130004918/234175517-c127edae-7eaa-4c7f-a926-6d36f443a9f1.png)

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

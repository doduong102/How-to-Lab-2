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

At first I was confused as to why the website was empty and I thought it wasn't working. But soon realized that it's because I originally populated the website with an empty string. I added a starting string is called from the handleRequest method. Also the main method is keeping this server up in an infinite loop. We know this because your terminal becomes unusable while the server is running and when you shut down your terminal the WebServer also stops functioning. 

Now in the url we can test our /add-message implementation

Copying this 'http://localhost:3010/add-message?s=Hello' into the url should yield:

![image](https://user-images.githubusercontent.com/130004918/234175432-473cee12-3dfe-4434-a447-05d4f5470146.png)

Which methods in your code are called?

`public static void main` is used to run the server given a port number.

`handleRequest` performs all the the commands we want out of the URL

What are the relevant arguments to those methods, and the values of any relevant fields of the class?

our 'main' method takes a string argument that will be used as the port of the server. Sometimes we cannot use a specific port because someone else on the same localhost has already taken it. 

`handleRequest` essentially "reads" through our URL. If the url is the same 
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

Once more with 'http://localhost:3010/add-message?s=Hey, Hi, Hello' should yield:
![image](https://user-images.githubusercontent.com/130004918/234175517-c127edae-7eaa-4c7f-a926-6d36f443a9f1.png)

Nice! Our basic implentation is working.

Which methods in your code are called?

`public static void main` is used to run the server given a port number.

`handleRequest` performs all the the commands we want out of the URL

What are the relevant arguments to those methods, and the values of any relevant fields of the class?

our `main` method takes a string argument that will be parsed into the port of the server. Sometimes we cannot use a specific port because someone else on the same localhost has already taken it. 

`handleRequest` essentially "reads" through our URL. If the url is unchanged and we press enter, `handleRequest` will basically just refresh the page. When we add `/add-message?s=Hello` our method will add our input the string following s= to our server in a new line. Our argument for 
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

# PART B| deBugGinG

![image](https://user-images.githubusercontent.com/130004918/234176128-f3412890-b350-4aae-a712-0dc7ccce099b.png)

WiP :')

# Part C| Reflections

![image](https://user-images.githubusercontent.com/130004918/234176285-6979e4d3-15af-475d-8b23-b793aae8dd8a.png)

WiP

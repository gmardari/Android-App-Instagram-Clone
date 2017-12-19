# Android-App-Instagram-Clone

A fun solo project with the goal of emulating a currently existing social networking app. 

<h2>Preview Images</h2>

Some images of development progress in chronological order:

https://imgur.com/hpl6Rnf

https://imgur.com/KIdZUVw

https://imgur.com/FfpZYmy

https://imgur.com/SzmFr3b

https://imgur.com/vabRCWz

https://imgur.com/VZJeWOL

<h2>Progress</h2>

Finished the basic networking system

Finished the feed

Finished sharing images function

Finished register/login and database functions

Finished the basic concept of the app, including image uploading, viewing, content retrieval, network events, uploading and downloading images from the server, user account database and content database (likes, shares, etc).  

<h2>Time for development</h2>
One week. (Did it during my break until I got busy)

<h2>Client Software Elements</h2>
Here are all the relevant client aspects of the program:

<h3>MainActivity.java</h3>
The main activity for the app. This handles connections and resources to the server through http requests. It requests content from the server using http, refreshes content automatically, and constructs different views for display on the screen. It stores the information regarding posts and content.

<h3>Network.java</h3>
Handles one network instance for every class to use. Handles all network functions using http requests and creates an easy to use interface for the rest of the program to interact with the server. It removes the need to implement the pain-stakingly long error checking anywhere else in the code, and puts all the data in JSON objects. It stores information such as user information, urls to services on the server, and the different network tasks (such as http requests) that are open.

<h3>HttpListener.java</h3>
A simple class to wait and listen on responses from the http requests sent by the network.

<h3>Functions.java</h3>
A class containing static functions for general use in the program.

<h3>State.java</h3>
Handles the functions for each state in the state machine by creating and removing views.

<h2>Server Software Elements</h2>

To view the Nodejs implementation of the backend for this app, see my repository Android-App-Instagram-Clone-Backend





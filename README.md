# Instant Messaging System

A messaging system allowing multiple clients to exchange and broadcast messages, as well as send files.

## How to run

Open the project in an IDE. Run `im_server/IMFrame.java` first. You should see the server menu printed on the terminal. Then you can run `im_client/IMView.java`. Use the usernames and passwords stored in `im_server/Server.java` to log in. You can log in to several clients to test out communication between them. To do that you may need to allow parallel run in the setting. <br><br>
All the usernames and passwords you can use to log in are:
```
Username, password
"100", "123456"
"200", "000000"
"Jack", "888888"
"Hank", "999999"
```

## Example

The screenshots below present an example of text communications between 1) server and client, 2) client and client.<br><br>
First, server is started and a message is sent to all the clients.<br><br>
<img src="./screenshot/imsystem_1.png" alt="server side menu" width="650"/>
<img src="./screenshot/imsystem_2.png" alt="server side sends a test message to all the clients" width="650"/><br><br>
And then, user 100 logs in and gets the message<br><br>
<img src="./screenshot/imsystem_client_1.png" alt="client side log-in interface" width="650"/>
<img src="./screenshot/imsystem_client_2.png" alt="user 100 logs in and receives the broadcast message" width="650"/><br><br>
User 200 logs in and gets the message, too. It then chooses to display the online user list. After seeing that only itself and user 100 are online, it sends a message "Hi 100, I am 200." to user 100, and the system tells it the message is sent.
<img src="./screenshot/imsystem_client_3.png" alt="user 200 logs in and gets the test message" width="650"/>
<img src="./screenshot/imsystem_client_4.png" alt="user 200 views the online user list" width="450"/><br>
<img src="./screenshot/imsystem_client_5.png" alt="user 200 sends the message" width="450"/><br><br>
And user 100 receives the message from 200 instantly.<br><br>
<img src="./screenshot/imsystem_client_6.png" alt="user 100 gets the message from 200" width="450"/>

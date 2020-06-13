---
layout: post
title: "Linux tricks and tips for beginners"
author: puneeth
categories: [Linux, Tutorial]
image: assets/images/chromeos/install-chrome-os.jpg
tags: [Linux, beginner, os]
---

Many of us use Linux, we mostly use Ubuntu which is beginner friendly with a good UI.

+ We should use commands in linux to get the full taste and to enjoy it.

#### 1. A small chat in Terminal:
When ever you are in a local connection, you might want a small session in terminal to connect with your friend, here comes `nc` command.
To begin with, assume one member as host and the other as a client.
The **host** should start the connection with the below command.
``` bash
nc -l 2222
```
- nc - netcat
- l  - Listen for an incoming connection.
- 2222- A port number. You can use any port number, randomly try a 4 digit, if it fails saying it is in use try another..

The client should enter below command.
``` bash
nc -l 192.168.102.73 2222
```
`192.168.102.73` is the IP address of the host. Check the IP address of the host by typing `ifconfig` command and finally enter the port number.

That's it!! you are now connected. You can send the text messages..
If you want to terminate the session press `CTRL + c`

#### 2. History clear:
History in Terminal is Handy thing, but for some users want to clear it.
We can clear the history by
``` bash
history -c
```

#### 3. Manual or Help:
To get the manual or docs for a command 
```
man nc
```
which ever command you want type it after `man`.

#### 4. sudo:
Sudo is a super user command used to passing the command as a super user.
```bash
sudo gedit test.py
```
<p align="center">
  <img width="45%" style="border:0.5px solid black" alt="Sudo meme" src="{{site.baseurl}}/assets/images/linux/sudo-meme.jpeg">
</p>

<p align="center">
  <img width="45%" style="border:0.5px solid black" alt="Sudo meme" src="{{site.baseurl}}/assets/images/linux/sudo-meme-1.jpg">
</p>

#### 5. Shutdown and Restart:
If you are a keyboard user 
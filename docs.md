---
layout: page
title: Docs
permalink: /docs/
---

* [Accessing the server](#access_server)
* [Simple guide to SSH](#ssh)
* [Setting up your webpage](#setup_webpage)
* [Uploading Files](#upload)
* [Simple intro to Filezilla](#filezilla)

### Accessing the server<a name="access_server"></a>

You will have received your account info in an email from the society. If you have not gotten this email or you are not signed up to the society, you can email internet.society@ucd.ie or contact us through the [UCD Netsoc Facebook group](https://facebook.com/ucdnetsoc).

To use your account, you have to log in using SSH and on your first login, you will be prompted to enter a new password. You might have to log in again once you have set your new password.

### Simple guide to SSH<a name="ssh"></a>

To administer your account on the server, you need to log in using SSH (Secure shell)
An SSH client should be available by default on Mac and Linux.
It might already be available on Windows, but if not, we recommend using the Putty SSH client.

To connect to the server, open a terminal/console and type:

` ssh username@netsoc.ucd.ie `

You should now be prompted for your password.

` username@netsoc.ucd.ie's password: `

(Don't worry if it's not displaying anything as you type in your password. That's how it's supposed to work)

If you're using Putty, just open the program and fill in the blanks

![Image showing how to connect to server using Putty](/images/putty_guide.png)

### Setting up your webpage<a name="setup_webpage"></a>

You will by default have a webpage setup at the URL: netsoc.ucd.ie/~_"student_id". Use the following command to change the URL, for example to netsoc.ucd.ie/~cool_page. The ~ is mandatory.

` rename_my_page cool_page `

To set up a basic webpage, simply add a file called index.html to the www/ folder in your home directory on the server. The contents of that index.html file will then be displayed with the address netsoc.ucd.ie/~pagename

To create your website, you can use whichever framework you want! Or you could open up your favourite text editor and W3schools’s Intro to HTML and CSS, and start coding away!

If there are features you want on your website that we currently don’t support, please tell us and we’ll do our best to accommodate you.

### Uploading files<a name="upload"></a>

Here are a few simple ways to get your files from your computer to your server. In these examples, I'll send a file called index.html to the folder /www/ in my home directory on the server.

Most SSH clients support SFTP(SSH File Transfer Protocol), which allows you to use the terminal/console to send files to the server.

If you just want to send a single file to the server, you can use:

` scp index.html username@netsoc.ucd.ie:www/ `

If you want to transfer multiple files, you could use SFTP in the terminal, but we recommend using a client like FileZilla in this case. (Remember to avoid installing Bing search and Opera when downloading FileZilla)


### Here's a simple introduction to FileZilla.<a name="filezilla"></a>

Connect to the netsoc.ucd.ie host with your username and password. Remember to set the port to 22 (to use SFTP).

![Image showing how to connect to server using FileZilla](/images/filezilla_login.png)

The window on the right displays your current folder on the server(top) and the contents of that folder(bottom).

![Image showing how files are shown in FileZilla](/images/filezilla_server_files.png)

You can navigate using the top window to find the location where you want to upload a file then either find your file in the left window or in a separate file explorer and drag it to somewhere in the right window. Your file should now be uploaded to the server in the location you dragged it to.

![Image showing how to drag files to send them with FileZilla](/images/filezilla_drag_drop.png)
### Installing Apache Web Server
Step 1

First of all, make sure to update the package list on your Raspberry Pi by entering the following commands.


    sudo apt-get update -y && sudo apt-get upgrade
  
Step 2

Then install Apache2 package by entering the following command

    sudo apt install apache2 -y

That’s it! Just two steps and you have an Apache Web Server up and running on your Raspberry Pi!
To confirm whether this web server is running or not, enter the following command.

    sudo service apache2 status

Now, in order to check that Apache is running, you can enter the IP address of your Raspberry Pi on a web browser and you will be presented with a simple web page as hown below. If you don’t know the IP address of your Raspberry Pi, you can find it by entering the command below in the terminal of your Raspberry Pi.

    hostname -I
![apache2_homepage](https://github.com/Binzv/Raspberry-pi-zero/assets/51468189/0a145fc4-0f63-48f1-b5a4-b17c2cf12720)

### 3. Setting up HTML page for editing
The default web page as shown above is just an HTML file on the filesystem of the Raspberry Pi. We will create our own HTML file and build our own webpage.

Step 1

First, let’s find the location of this HTML file on the Raspberry Pi. Enter the following command in the terminal

    cd /var/www/html 
Step 2

Then type the following command to list all the files in this directory

    ls -al



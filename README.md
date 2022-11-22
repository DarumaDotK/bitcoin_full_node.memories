# bitcoin-fullnode.memories
 Usage and Troubleshooting Logs of Running Bitcoin Full Node
 
## Minimum Requirements

- Desktop or laptop hardware running recent versions of Windows, Mac OS X, or Linux.
- 7 gigabytes of free disk space, accessible at a minimum read/write speed of 100 MB/s.
- 2 gigabytes of memory (RAM)
- A broadband Internet connection with upload speeds of at least 400 kilobits (50 kilobytes) per second
- An unmetered connection, a connection with high upload limits, or a connection you regularly monitor to ensure it doesn’t exceed its upload limits. It’s common for full nodes on high-speed connections to use 200 gigabytes upload or more a month. Download usage is around 20 gigabytes a month, plus around an additional 340 gigabytes the first time you start your node.
- 6 hours a day that your full node can be left running. (You can do other things with your computer while running a full node.) More hours would be better, and best of all would be if you can run your node continuously.

**NOTE** : many operating systems today (Windows, Mac, and Linux) enter a low-power mode after the screensaver activates, slowing or halting network traffic. This is often the default setting on laptops and on all Mac OS X laptops and desktops. Check your screensaver settings and disable automatic “sleep” or “suspend” options to ensure you support the network whenever your computer is running.

## Install Bitcoin Full Node

First you open your Terminal and use the command line :

~~~
sudo apt update && sudo apt upgrade -y
~~~

then install snap package manager. [more](https://snapcraft.io/docs/installing-snapd)

~~~
sudo apt install snapd
~~~

then install bitcoin-core

~~~
sudo snap install bitcoin-core
~~~

![pic1](/src/Screenshot%20from%202022-11-22%2015-43-28.png)

Check the version and complete installation.

![pic2](/src/Screenshot%20from%202022-11-22%2015-44-04.png)

~~~
bitcoin-core.cli --version
~~~

![pic3](/src/Screenshot%20from%202022-11-22%2015-44-16.png)

Open Activities. You will find a bitcoin icon. double click it

![pic4](/src/Screenshot%20from%202022-11-22%2015-44-38.png)

Unless you plan on configuring anything else. You can use the default. The important part of this step is the path. `/home/devg/snap/bitcoin-core/common/.bitcoin` Click "Next" to continue.

![pic5](/src/Screenshot%20from%202022-11-22%2015-45-25.png)

Complete the installation. Then you just wait for the sync to 100%.

![pic6](/src/Screenshot%20from%202022-11-22%2015-46-00.png)

## uninstall bitcoin-core

~~~
sudo snap remove bitcoin-core
~~~
